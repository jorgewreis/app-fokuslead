# TAP - Anexo 11: Documento de Requisitos de Software (DRS)

## Metadados

- **Projeto:** FokusLead
- **Documento:** TAP - Anexo 11: Documento de Requisitos de Software (DRS)
- **Versão:** 1.01
- **Responsável:** Jorge Reis
- **Data:** Atual

## Documentos relacionados

- `docs/documents/tap/doc-tap-01-stakeholders.md`
- `docs/documents/tap/doc-tap-02-gerenciamento-escopo.md`
- `docs/documents/tap/doc-tap-03-gerenciamento-riscos.md`
- `docs/documents/tap/doc-tap-04-gerenciamento-custos.md`
- `docs/documents/tap/doc-tap-05-gerenciamento-qualidade.md`
- `docs/documents/tap/doc-tap-06-cronograma-marcos.md`
- `docs/documents/tap/doc-tap-07-estrutura-analitica-projeto-eap.md`
- `docs/documents/tap/doc-tap-08-guia-funcionalidades.md`
- `docs/documents/tap/doc-tap-09-guia-implementacao-roadmap-semestral.md`
- `docs/documents/tap/doc-tap-10-modelo-comercial-planos-assinatura.md`
- `docs/documents/charter/doc-charter-01-termo-abertura-projeto.md`

## Prefácio

### Histórico de versões

| Versão | Data | Autor | Descrição |
| --- | --- | --- | --- |
| 1.01 | Atual | Jorge Reis | Atualização completa com visão do produto full. |

## 1. Introdução

### 1.1 Objetivo

Este Documento de Requisitos de Software (DRS) define as necessidades, restrições e funcionalidades do FokusLead, servindo como registro formal e base de entendimento entre cliente e equipe técnica. O documento cobre a visão completa do produto, desde a base imobiliária até a plataforma escalável para equipes.

### 1.2 Escopo do software

O FokusLead é um CRM imobiliário multiplataforma que centraliza leads, clientes, imóveis e interações, apoiando o processo comercial completo de corretores e imobiliárias. O sistema integra canais externos (WhatsApp e Instagram), organiza o funil de vendas e oferece indicadores para tomada de decisão.

### 1.3 Público-alvo

- Corretores de imóveis (FokusLead One)
- Imobiliárias e equipes comerciais (FokusLead Team)

### 1.4 Definições e siglas

- **CRM:** Customer Relationship Management
- **DRS/SRS:** Documento de Requisitos de Software
- **EAP/WBS:** Estrutura Analítica do Projeto
- **LGPD:** Lei Geral de Proteção de Dados
- **PWA:** Progressive Web App

## 2. Glossário

- **Lead:** contato inicial com potencial cliente, sem qualificação completa.
- **Cliente:** pessoa com cadastro estruturado e histórico de interações.
- **Imóvel:** ativo comercial com atributos de venda e disponibilidade.
- **Funil de vendas:** etapas que representam a evolução de uma oportunidade.
- **Oportunidade:** relação comercial em andamento entre cliente e imóvel.

## 3. Requisitos do usuário

- Registrar imóveis, empreendimentos, construtoras e dados de localização.
- Captar e organizar leads de múltiplos canais com histórico completo.
- Classificar clientes e leads por tags, prioridade e perfis.
- Controlar funil de vendas e visualizar pipeline.
- Agendar visitas, retornos e follow-ups com lembretes.
- Receber indicadores de desempenho comercial.
- Gerenciar equipes e permissões (Team).

## 4. Arquitetura do sistema (visão macro)

- Backend centralizado com regras de negócio unificadas.
- Interface web responsiva e evolução para PWA e apps móveis.
- Camada de integração desacoplada para APIs externas.
- Banco de dados relacional com trilhas de auditoria e histórico.

## 5. Especificação de requisitos

### 5.1 Requisitos funcionais

- **RF-01:** Permitir autenticação de usuários com controle de sessão.
- **RF-02:** Permitir recuperação de senha com token temporário.
- **RF-03:** Permitir cadastro de construtoras e incorporadoras.
- **RF-04:** Permitir cadastro de empreendimentos vinculados a construtoras.
- **RF-05:** Permitir cadastro de imóveis e tipos de imóveis.
- **RF-06:** Permitir cadastro de cidades e bairros com vínculo obrigatório.
- **RF-07:** Permitir cadastro de clientes com histórico de interações.
- **RF-08:** Permitir registro de leads com origem e data de entrada.
- **RF-09:** Permitir conversão de lead em cliente preservando histórico.
- **RF-10:** Permitir registro de interações (mensagens, notas e ligações).
- **RF-11:** Permitir relacionamento N:N entre clientes e imóveis.
- **RF-12:** Permitir funil de vendas com etapas configuráveis.
- **RF-13:** Permitir criação e gestão de oportunidades comerciais.
- **RF-14:** Permitir agenda comercial com visitas e follow-ups.
- **RF-15:** Permitir matching entre perfil do cliente e imóveis compatíveis.
- **RF-16:** Permitir indicadores de desempenho (leads, conversões, tempo de resposta).
- **RF-17:** Permitir integração com WhatsApp Business API.
- **RF-18:** Permitir integração com Instagram API.
- **RF-19:** Permitir gestão de usuários, perfis e permissões (Team).
- **RF-20:** Permitir logs de acesso e rastreabilidade básica.

### 5.2 Requisitos não funcionais

- **RNF-01:** Garantir tempo de resposta de até 2 segundos nas telas principais.
- **RNF-02:** Garantir disponibilidade mínima de 99% mensal.
- **RNF-03:** Garantir criptografia de dados sensíveis em trânsito e repouso.
- **RNF-04:** Garantir conformidade com LGPD (consentimento e minimização).
- **RNF-05:** Garantir escalabilidade para aumento de usuários e leads.
- **RNF-06:** Garantir compatibilidade com navegadores modernos e PWA.
- **RNF-07:** Garantir logs de auditoria para ações críticas.
- **RNF-08:** Garantir backups regulares e recuperação de dados.

### 5.3 Requisitos de domínio

- **RD-01:** Exigir vínculo obrigatório entre empreendimentos e construtoras.
- **RD-02:** Exigir vínculo obrigatório entre bairros e cidades.
- **RD-03:** Permitir múltiplos imóveis por cliente e múltiplos clientes por imóvel.
- **RD-04:** Preservar histórico de leads convertidos em clientes.
- **RD-05:** Respeitar políticas de uso e limites das APIs externas.

## 6. Modelos do sistema

Os diagramas estao organizados por tipo em `docs/diagrams`, com fontes em PlantUML e imagens por categoria.

Casos de uso:

- `docs/diagrams/use-cases/plantuml/diag-uc-01-fokuslead-mvp.puml`

Diagramas de classes (modelos conceituais):

- `docs/diagrams/classes/plantuml/diag-class-02-camada-nucleo-usuario.puml`
- `docs/diagrams/classes/plantuml/diag-class-03-estrutura-imobiliaria.puml`
- `docs/diagrams/classes/plantuml/diag-class-04-gestao-comercial.puml`
- `docs/diagrams/classes/plantuml/diag-class-05-funil-vendas.puml`
- `docs/diagrams/classes/plantuml/diag-class-06-comunicacao-produtividade.puml`
- `docs/diagrams/classes/plantuml/diag-class-07-integracoes-auditoria.puml`
- `docs/diagrams/classes/plantuml/diag-class-08-visao-geral-conceitual.puml`
- `docs/diagrams/classes/plantuml/diag-class-13-diagrama-classes.puml`

Diagramas de sequencia:

- `docs/diagrams/sequence/plantuml/diag-seq-01-captura-lead-whatsapp.puml`
- `docs/diagrams/sequence/plantuml/diag-seq-02-captura-lead-instagram.puml`
- `docs/diagrams/sequence/plantuml/diag-seq-03-login-google.puml`
- `docs/diagrams/sequence/plantuml/diag-seq-04-conversao-lead-cliente.puml`
- `docs/diagrams/sequence/plantuml/diag-seq-05-mudanca-etapa-funil.puml`
- `docs/diagrams/sequence/plantuml/diag-seq-09-captura-lead-whatsapp-basico.puml`

Diagrama de atividade:

- `docs/diagrams/activity/plantuml/diag-ativ-01-ciclo-lead.puml`
- `docs/diagrams/activity/plantuml/diag-ativ-10-funil-vendas.puml`

Diagrama de estados:

- `docs/diagrams/states/plantuml/diag-state-11-imovel.puml`

Diagrama de componentes:

- `docs/diagrams/components/plantuml/diag-comp-12-integracoes.puml`

Diagrama de implantacao:

- `docs/diagrams/deployment/plantuml/diag-deploy-01-aws.puml`

## 7. Evolução e apêndices

- O controle de escopo está definido no `docs/documents/tap/doc-tap-02-gerenciamento-escopo.md`.
- O detalhamento de funcionalidades por domínio está no `docs/documents/tap/doc-tap-08-guia-funcionalidades.md`.
- A evolução do produto segue os módulos definidos no `docs/documents/tap/doc-tap-09-guia-implementacao-roadmap-semestral.md`.






