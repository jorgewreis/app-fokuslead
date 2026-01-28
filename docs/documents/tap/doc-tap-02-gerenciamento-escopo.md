# TAP - Anexo 2: Gerenciamento de Escopo

## Metadados

- **Projeto:** FokusLead
- **Documento:** TAP - Anexo 2: Gerenciamento de Escopo
- **Versão:** 1.01
- **Responsável:** Jorge Reis
- **Data:** Atual

## Documentos relacionados

- `docs/documents/tap/doc-tap-01-stakeholders.md`
- `docs/documents/tap/doc-tap-03-gerenciamento-riscos.md`
- `docs/documents/tap/doc-tap-04-gerenciamento-custos.md`
- `docs/documents/tap/doc-tap-05-gerenciamento-qualidade.md`
- `docs/documents/tap/doc-tap-06-cronograma-marcos.md`
- `docs/documents/tap/doc-tap-07-estrutura-analitica-projeto-eap.md`
- `docs/documents/tap/doc-tap-08-guia-funcionalidades.md`
- `docs/documents/tap/doc-tap-09-guia-implementacao-roadmap-semestral.md`
- `docs/documents/tap/doc-tap-10-modelo-comercial-planos-assinatura.md`
- `docs/documents/tap/doc-tap-11-documento-requisitos-software-drs.md`
- `docs/documents/charter/doc-charter-01-termo-abertura-projeto.md`

## 1. Introdução e objetivo do gerenciamento de escopo

Este documento estabelece o Gerenciamento de Escopo do Projeto FokusLead em sua visão completa, contemplando desde a concepção inicial do sistema imobiliário até a consolidação da plataforma como CRM imobiliário escalável, conforme definido no `docs/documents/charter/doc-charter-01-termo-abertura-projeto.md`. O gerenciamento de escopo tem como finalidade assegurar que o projeto contemple todo o trabalho necessário para entregar o valor esperado ao mercado, sem incluir esforços não planejados, prevenindo expansão indevida de funcionalidades, desalinhamento estratégico e riscos à sustentabilidade técnica e comercial do produto.

Este anexo atua como referência oficial para:

- Definição do que compõe o produto FokusLead em sua totalidade.
- Delimitação clara entre funcionalidades atuais, futuras e excluídas.
- Controle de mudanças ao longo dos ciclos de evolução.
- Validação e aceitação das entregas em cada módulo do roadmap.

## 2. Definição do escopo do projeto

### 2.1 FokusLead (escopo incluído)

O escopo do projeto FokusLead abrange o desenvolvimento de uma plataforma digital de gestão comercial imobiliária, concebida para organizar dados, centralizar leads, estruturar o processo de vendas e fornecer visão gerencial para corretores e imobiliárias.

Estão incluídos no escopo global do projeto:

- Plataforma SaaS multiplataforma, com acesso via:
  - Web Desktop
  - Web Mobile
  - PWA
  - Aplicativos nativos iOS e Android (em fases posteriores)
- Arquitetura única de backend, com base de dados centralizada e regras de negócio unificadas.
- Evolução modular do produto em ciclos semestrais.
- Separação clara entre produto individual (FokusLead One) e produto corporativo (FokusLead Team).

### 2.2 FokusLead One (escopo funcional)

O FokusLead One contempla funcionalidades voltadas à produtividade individual do corretor, organizadas progressivamente ao longo do roadmap.

Inclui-se no escopo funcional do FokusLead One:

- Cadastro e gestão de:
  - Construtoras e incorporadoras
  - Empreendimentos imobiliários
  - Imóveis e tipos de imóveis
  - Clientes e leads
- Gestão estruturada de leads, com:
  - Captação via WhatsApp e Instagram
  - Registro de origem, data e canal
- Histórico completo de interações com clientes
- Classificação de clientes por perfis e tags
- Relacionamento entre clientes e imóveis de interesse
- Funil de vendas com etapas configuráveis
- Agenda comercial e controle de follow-ups
- Matching entre perfil do cliente e portfólio de imóveis
- Indicadores básicos de desempenho comercial
- Gestão do portfólio ativo de imóveis
- Segurança da informação e conformidade com LGPD

### 2.3 FokusLead Team (escopo funcional)

O FokusLead Team amplia o escopo do produto para operações com múltiplos usuários, atuando como camada de governança comercial.

Inclui-se no escopo do FokusLead Team:

- Gestão de múltiplos usuários
- Controle de permissões e hierarquias
- Gestão unificada de leads por equipe
- Padronização do processo comercial
- Dashboards gerenciais consolidados
- Indicadores comparativos por corretor e equipe
- Gestão centralizada do portfólio
- Auditoria básica, logs e rastreabilidade
- Suporte à escalabilidade operacional

## 3. Escopo excluído do projeto

Estão explicitamente fora do escopo do projeto FokusLead:

- Atuação como marketplace imobiliário
- Intermediação financeira ou cobrança de comissões
- Assinatura digital de contratos imobiliários
- Gestão jurídica de escrituras ou registros cartoriais
- Processamento de pagamentos de terceiros
- Integrações com plataformas não previstas no roadmap estratégico
- Desenvolvimento sob medida para clientes específicos fora do modelo SaaS

## 4. Engenharia de requisitos

### 4.1 Requisitos funcionais

O sistema FokusLead deverá permitir, ao longo de sua evolução:

- Cadastro completo de entidades imobiliárias
- Criação, gestão e qualificação de leads
- Centralização de interações multicanal
- Organização do funil de vendas
- Classificação avançada de clientes
- Relacionamento dinâmico cliente x imóvel
- Gestão de compromissos comerciais
- Visualização de indicadores de desempenho
- Administração de usuários e equipes (Team)
- Controle de acesso e permissões
- Operação contínua em múltiplas plataformas

### 4.2 Requisitos não funcionais

O projeto deverá atender, de forma contínua:

- Segurança e LGPD, com consentimento, anonimização e proteção de dados
- Performance, garantindo tempos de resposta adequados mesmo com crescimento de base
- Escalabilidade, permitindo aumento de usuários, dados e integrações
- Usabilidade, priorizando simplicidade e baixo atrito operacional
- Disponibilidade, com foco em uso diário e crítico para vendas

## 5. Regras de negócio globais

As principais regras de negócio do FokusLead incluem:

- Empreendimentos devem estar vinculados a construtoras e incorporadoras
- Imóveis do tipo apartamento exigem vínculo com empreendimento
- Clientes podem se relacionar com múltiplos imóveis
- Imóveis podem possuir múltiplos interessados
- Leads evoluem para clientes, preservando histórico
- Perfis e tags são configuráveis
- A lógica de negócio é centralizada no backend
- Limites de uso são definidos por plano de assinatura

## 6. Estrutura Analítica do Projeto (EAP / WBS)

O projeto é estruturado de forma hierárquica e modular.

- **Nível superior:** Projeto FokusLead
- **Nível intermediário:** módulos evolutivos alinhados ao roadmap semestral
- **Níveis inferiores:** pacotes de trabalho funcionais e técnicos, contemplando desenvolvimento, integração, testes, validação e documentação

Essa estrutura permite controle de escopo, planejamento progressivo e evolução segura do produto. A definição detalhada está no `docs/documents/tap/doc-tap-07-estrutura-analitica-projeto-eap.md`.

## 7. Dicionário da EAP

Cada pacote de trabalho do projeto deverá possuir definição clara contendo:

- Descrição funcional
- Entregáveis esperados
- Critérios objetivos de aceitação
- Dependências técnicas
- Responsável pela execução

O Dicionário da EAP é instrumento obrigatório para evitar ambiguidades e garantir alinhamento entre visão estratégica e execução técnica.

## 8. Critérios de aceitação do escopo

O projeto FokusLead será considerado entregue de forma satisfatória quando:

- Cada módulo do roadmap for concluído conforme escopo aprovado
- As funcionalidades entregues atenderem aos requisitos definidos
- O sistema operar de forma estável, seguro e usável
- O produto gerar valor perceptível aos usuários
- Não houver funcionalidades críticas fora do controle de escopo

## 9. Controle de escopo e gestão de mudanças

Qualquer solicitação que implique impacto em escopo, prazo, custo ou arquitetura deverá ser formalmente avaliada.

As mudanças podem:

- Ser aprovadas e incorporadas ao módulo atual
- Ser postergadas para módulos futuros
- Ser rejeitadas por desalinhamento estratégico

Nenhuma alteração deve ser implementada sem análise prévia de impacto.

## 10. Gestão de exclusões e histórico

O sistema deverá preservar integridade histórica dos dados. Exclusões físicas serão controladas quando houver dependências relevantes. Históricos comerciais relevantes deverão ser preservados por meio de registros mínimos, garantindo rastreabilidade e coerência do processo comercial.

## 11. Riscos relacionados ao escopo

Os principais riscos associados ao escopo incluem:

- Expansão indevida de funcionalidades
- Pressão por entregas fora do roadmap
- Dependência excessiva de integrações externas
- Complexidade técnica antecipada

A mitigação ocorrerá por meio de:

- Desenvolvimento modular
- Validação contínua
- Governança clara
- Documentação consistente

## 12. Integração com o TAP e documentos complementares

Este anexo integra-se diretamente aos seguintes documentos:

- `docs/documents/tap/doc-tap-01-stakeholders.md`
- `docs/documents/tap/doc-tap-08-guia-funcionalidades.md`
- `docs/documents/tap/doc-tap-09-guia-implementacao-roadmap-semestral.md`
- `docs/documents/charter/doc-charter-01-termo-abertura-projeto.md`

Atua como documento estruturante do projeto, orientando execução, controle e evolução do FokusLead em sua totalidade.


