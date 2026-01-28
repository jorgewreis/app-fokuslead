# TAP - Anexo 12: Arquitetura e Tecnologias

## Metadados

- **Projeto:** FokusLead
- **Documento:** TAP - Anexo 12: Arquitetura e Tecnologias
- **Versão:** 1.0
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

- **Apresentação:** Next.js (SSR + páginas web)
- **Aplicação:** casos de uso e orquestração de fluxos
- **Domínio:** entidades e regras centrais do negócio
- **Infraestrutura:** banco, integrações, cache, mensageria futura

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

### 6.5 CI/CD

- **Ferramenta:** GitHub Actions

### 6.6 Observabilidade

- **Logs, métricas e alertas:** AWS CloudWatch

## 7. Segurança e LGPD

- **Criptografia em trânsito:** HTTPS/TLS
- **Backups:** diários com retenção de 30 dias
- **Logs e auditoria:** registrados para ações críticas
- **Anonimização:** prevista para dados sensíveis conforme LGPD

## 8. Autenticação e autorização

- **Autenticação:** JWT
- **Autorização:** RBAC (papéis e permissões)

## 9. Integrações externas

- **WhatsApp Business API**
- **Instagram API**

## 10. Estratégia de testes

- **Testes unitários:** obrigatórios
- **Testes de integração:** obrigatórios
- **Testes E2E:** fluxos críticos
- **Cobertura mínima:** 70% unitários, 50% integração
- **Testes de carga:** previstos para fases futuras

## 11. Padrões de código e qualidade

- **Lint/format:** TBD
- **Padrão de commits:** TBD
- **Versionamento:** TBD

## 12. Riscos técnicos e mitigação

- Dependência de APIs externas (WhatsApp/Instagram) e suas políticas.
- Crescimento exponencial pode exigir extração modular futura.
- Operação em AWS demanda curva de aprendizado inicial.

## 13. Itens em aberto

- Definição de lint/format e padrão de commits.
- Estratégia detalhada de deploy em AWS.
- Política detalhada de logs e auditoria por domínio.

