# TAP - Anexo 12: Arquitetura e Tecnologias

## Metadados

- **Projeto:** FokusLead
- **Documento:** TAP - Anexo 12: Arquitetura e Tecnologias
- **Versão:** 1.01
- **Responsável:** Jorge Reis
- **Data:** 28/01/2026
- **Público-alvo:** Desenvolvedores internos
- **Nível de detalhamento:** Profundo

## 1. Objetivo

Este documento define a arquitetura de software e o conjunto de tecnologias adotado no FokusLead, estabelecendo diretrizes técnicas para construção, evolução e operação do produto com foco em velocidade de entrega inicial e escalabilidade futura.

## 2. Princípios e direcionadores

- Entrega rápida com base sólida para evolução.
- Simplicidade operacional no início (equipe de 1 pessoa).
- Modularidade para permitir extrações futuras.
- Observabilidade mínima obrigatória desde o começo.
- Segurança e LGPD como requisitos centrais.

## 3. Estilo arquitetural

### 3.1 Escolha principal

- **Monólito modular com princípios de Clean Architecture.**

### 3.2 Justificativa

- Minimiza complexidade operacional inicial.
- Acelera desenvolvimento com baixo custo de infraestrutura.
- Mantém separação de domínios e facilita testes.
- Permite migração gradual para microserviços quando necessário.

### 3.3 Estratégia de evolução

- Organizar o código por domínios (módulos).
- Definir contratos claros entre camadas.
- Identificar domínios candidatos à extração futura (ex.: integrações, notificações).
- Adotar eventos internos para reduzir acoplamento.

## 4. Visão geral de arquitetura (macro)

- Backend centralizado com regras de negócio unificadas.
- Frontend web SSR para entrega rápida e boa experiência inicial.
- Camada de integração desacoplada para APIs externas.
- Banco relacional com auditoria e trilha histórica.
- Cache e logs complementares via Redis.

## 5. Camadas e componentes

### 5.1 Camadas lógicas

- **Apresentação:** controllers/UI; valida entrada e aciona casos de uso.
- **Aplicação:** casos de uso; orquestra fluxos e regras do domínio.
- **Domínio:** entidades e serviços de domínio; invariantes do negócio.
- **Infraestrutura:** repositórios/adapters; banco, integrações, cache, serviços externos.

### 5.2 Serviços e módulos internos (monólito)

- Autenticação e autorização
- Cadastros (imóveis, clientes, leads, empreendimentos)
- Funil de vendas e oportunidades
- Interações e histórico
- Integrações externas (WhatsApp/Instagram)
- Auditoria e logs

## 6. Tecnologias definidas

### 6.1 Backend

- **Linguagem:** Node.js
- **Framework:** NestJS
- **Padrões:** Clean Architecture (camadas bem definidas)
- **ORM:** Prisma

### 6.2 Frontend

- **Framework:** Next.js
- **Abordagem:** SSR (Server-Side Rendering)
- **PWA:** previsto para evolução futura

### 6.3 Banco de dados e cache

- **SGBD principal:** MySQL
- **Cache/Logs:** Redis

### 6.4 Infraestrutura

- **Cloud:** AWS
- **Containerização:** Docker (com Docker Compose no início)
- **Orquestração futura:** ECS (quando houver necessidade)

### 6.5 Estratégia de deploy em AWS

- **Execução:** ECS Fargate para backend em containers gerenciados.
- **Banco:** RDS MySQL com backups automatizados e alta disponibilidade.
- **Balanceamento:** Application Load Balancer (ALB) com HTTPS.
- **Assets estáticos:** S3 + CloudFront para distribuição de frontend/arquivos.
- **Rede:** VPC com subnets privadas; apenas o ALB exposto publicamente.
- **Segredos:** AWS Secrets Manager para credenciais e chaves.
- **Pipeline:** GitHub Actions com build, testes e push para ECR.

### 6.6 CI/CD

- **Ferramenta:** GitHub Actions

### 6.7 Observabilidade

- **Logs, métricas e alertas:** AWS CloudWatch

### 6.8 Política de logs e auditoria por domínio

- **Autenticação e autorização:** login/logout, falhas, reset de senha, mudanças de papel/permissão.
- **Cadastros:** criação/edição/exclusão de imóveis, clientes, leads e empreendimentos.
- **Funil e oportunidades:** mudança de estágio, ganho/perda, atribuição de responsável.
- **Interações e histórico:** registros de contato, notas e anexos.
- **Integrações externas:** webhooks recebidos/enviados, falhas, retries e status de sincronização.
- **Configurações e auditoria:** alterações em integrações, parâmetros de sistema e usuários.
- **Campos mínimos:** usuário, data/hora, entidade afetada, ação, antes/depois, origem (IP/dispositivo).
- **Regras:** logs sem dados sensíveis; auditoria imutável e consultável por perfil autorizado.
- **Retenção:** logs operacionais por 30 dias; auditoria por 6 meses.
- **Armazenamento:** tabela de auditoria imutável com índice por data, usuário e entidade.
- **Acesso:** consulta por período, usuário e entidade; exportação para CSV com permissão.

## 7. Segurança e LGPD

- **Criptografia em trânsito:** HTTPS/TLS
- **MFA:** autenticação multifator via SMS
- **IAM por função:** acesso mínimo necessário por perfis de infraestrutura
- **Criptografia em repouso:** banco, backups e arquivos armazenados
- **WAF:** proteção contra ataques comuns (SQLi, XSS, bots)
- **Backups:** diários com retenção de 30 dias
- **Logs e auditoria:** registrados para ações críticas
- **Anonimização:** prevista para dados sensíveis conforme LGPD

## 8. Autenticação e autorização

- **Autenticação:** JWT
- **Autorização:** RBAC (papéis e permissões)

## 9. Integrações externas

- **WhatsApp Business API**
- **Instagram API**

### 9.1 Detalhamento das integrações (Meta)

- **APIs:** WhatsApp Business Cloud API e Instagram Graph API.
- **Autenticação:** OAuth 2.0 com tokens gerenciados e renovação periódica.
- **Webhooks:** assinatura de eventos e validação de assinatura nas requisições recebidas.
- **Limites e políticas:** respeito a rate limits, termos de uso e políticas de conteúdo.
- **Aprovação:** configuração de app e revisão de permissões na plataforma Meta.
- **Privacidade:** tratamento de dados conforme LGPD e consentimento quando aplicável.

## 10. Estratégia de testes

- **Testes unitários:** obrigatórios
- **Testes de integração:** obrigatórios
- **Testes E2E:** fluxos críticos
- **Cobertura mínima:** 70% unitários, 50% integração
- **Testes de carga:** previstos para fases futuras

## 10.1 Arquitetura de dados: modelagem

- **Modelo:** relacional normalizado (ER) com chaves estrangeiras.
- **Soft delete:** registros marcados como inativos para evitar perdas.
- **Histórico:** trilha de mudanças para auditoria e conformidade.

## 11. Padrões de código e qualidade

- **Lint/format:** ESLint
- **Padrão de commits:** Conforme `COMMITS.md` (formato `tipo: descrição`)
- **Versionamento:** V 1.00.00 (1a parte = release completa; 2a parte = grandes implementações; 3a parte = qualquer implementação ou correção). Ao atingir 99 na 3a parte, zera e incrementa a 2a parte. Em cada release, incrementa a 1a parte e zera as demais.
- **Automação:** hooks `commit-msg` + `post-commit` atualizam o arquivo `VERSION` conforme o tipo do commit.

## 12. Riscos técnicos e mitigação

- Dependência de APIs externas (WhatsApp/Instagram) e suas políticas.
- Crescimento exponencial pode exigir extração modular futura.
- Operação em AWS demanda curva de aprendizado inicial.
