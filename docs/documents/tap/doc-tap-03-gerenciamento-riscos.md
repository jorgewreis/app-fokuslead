# TAP - Anexo 3: Gerenciamento de Riscos

## Metadados

- **Projeto:** FokusLead
- **Documento:** TAP - Anexo 3: Gerenciamento de Riscos
- **Versão:** 1.01
- **Responsável:** Jorge Reis
- **Data:** Atual

## Documentos relacionados

- `docs/documents/tap/doc-tap-01-stakeholders.md`
- `docs/documents/tap/doc-tap-02-gerenciamento-escopo.md`
- `docs/documents/tap/doc-tap-04-gerenciamento-custos.md`
- `docs/documents/tap/doc-tap-05-gerenciamento-qualidade.md`
- `docs/documents/tap/doc-tap-06-cronograma-marcos.md`
- `docs/documents/tap/doc-tap-07-estrutura-analitica-projeto-eap.md`
- `docs/documents/tap/doc-tap-08-guia-funcionalidades.md`
- `docs/documents/tap/doc-tap-09-guia-implementacao-roadmap-semestral.md`
- `docs/documents/tap/doc-tap-10-modelo-comercial-planos-assinatura.md`
- `docs/documents/tap/doc-tap-11-documento-requisitos-software-drs.md`
- `docs/documents/charter/doc-charter-01-termo-abertura-projeto.md`

## 1. Introdução e objetivo

Este documento tem como objetivo identificar, analisar, priorizar e definir estratégias de resposta aos principais riscos do Projeto FokusLead, considerando todo o ciclo evolutivo do produto, do sistema imobiliário estrutural até a plataforma escalável e multiusuário. O Gerenciamento de Riscos visa reduzir incertezas, antecipar problemas críticos e fornecer base estruturada para a tomada de decisão, assegurando maior previsibilidade e controle durante a execução do projeto.

Este anexo complementa o `docs/documents/charter/doc-charter-01-termo-abertura-projeto.md` e os demais documentos de planejamento, atuando como referência formal para monitoramento contínuo de riscos ao longo do ciclo de vida do produto.

## 2. Abordagem de gerenciamento de riscos

O projeto adota uma abordagem híbrida de gerenciamento de riscos, combinando:

- Prevenção ativa para riscos críticos ou de alto impacto
- Resposta planejada e monitoramento para riscos de menor severidade

Essa abordagem permite foco eficiente nos riscos mais relevantes, sem gerar sobrecarga operacional desnecessária.

## 3. Categorias de risco adotadas

Os riscos do projeto foram classificados nas seguintes categorias:

- Riscos técnicos
- Riscos de prazo
- Riscos de dependência externa
- Riscos de qualidade
- Riscos legais e LGPD
- Riscos comerciais e de adoção
- Riscos de escalabilidade

## 4. Metodologia de avaliação de riscos

### 4.1 Escala de avaliação

Cada risco é avaliado com base em dois critérios:

- **Probabilidade (1 a 5):**
  - 1 = Muito baixa
  - 5 = Muito alta
- **Impacto (1 a 5):**
  - 1 = Impacto mínimo
  - 5 = Impacto crítico para o programa

### 4.2 Cálculo do nível de risco

O nível de risco é determinado pela fórmula ponderada:

- **Nível de risco = (Probabilidade x 2) + (Impacto x 3)**

Essa ponderação atribui maior peso ao impacto, refletindo a criticidade de eventos que possam comprometer o prazo, a integridade do produto ou a conformidade legal. A pontuação final varia de 5 a 25, permitindo ordenação objetiva dos riscos.

## 5. Registro e avaliação dos riscos

| ID | Risco | Categoria | Prob. | Impacto | Nível | Estratégia | Ações principais |
| --- | --- | --- | --- | --- | --- | --- | --- |
| R1 | Mudança em APIs de terceiros | Dependência externa | 3 | 5 | 21 | Mitigar | Abstração de integrações e monitoramento de políticas. |
| R2 | Instabilidade em picos de uso | Técnico | 3 | 4 | 18 | Transferir | Infraestrutura gerenciada e escalável. |
| R3 | Falhas de autenticação e sessão | Técnico | 2 | 5 | 19 | Mitigar | Padrões consolidados e testes de segurança. |
| R4 | Dependência de gateways de cobrança | Dependência externa | 2 | 4 | 16 | Transferir | Serviços especializados para billing e assinatura. |
| R5 | Performance do frontend em dispositivos | Qualidade | 3 | 3 | 15 | Mitigar | Otimização de assets e testes de performance. |
| R6 | Consistência responsiva multiplataforma | Qualidade | 3 | 3 | 15 | Mitigar | Design system e testes em múltiplas resoluções. |
| R7 | Atraso no cronograma por escopo | Prazo | 3 | 4 | 18 | Mitigar | Controle formal de mudanças e priorização. |
| R8 | Exposição indevida de dados pessoais | Legal e LGPD | 2 | 5 | 19 | Mitigar | Controle de acesso, mascaramento e auditoria. |
| R9 | Experiência ruim em mobile e PWA | Qualidade | 3 | 3 | 15 | Mitigar | Testes de UX e validações frequentes. |
| R10 | Escalabilidade para operações Team | Escalabilidade | 3 | 4 | 18 | Mitigar | Arquitetura modular e testes de carga. |
| R11 | Qualidade de dados e duplicidades | Técnico | 4 | 3 | 17 | Mitigar | Regras de validação e deduplicação. |
| R12 | Baixa adesão ou churn precoce | Comercial | 3 | 4 | 18 | Mitigar | Evolução orientada a valor e onboarding assistido. |

## 6. Estratégias de resposta aos riscos

As estratégias de resposta seguem as diretrizes abaixo:

- **Mitigar:** reduzir probabilidade e impacto com ações preventivas.
- **Transferir:** delegar parte do risco a terceiros (infra, APIs, billing).
- **Aceitar:** monitorar e reagir quando o custo de mitigação for inviável.

## 7. Monitoramento e revisão dos riscos

O monitoramento dos riscos será contínuo e integrado ao acompanhamento do cronograma e do escopo do projeto, observando:

- Alterações no nível de risco
- Materialização de eventos previstos
- Necessidade de revisão de estratégias

Riscos críticos poderão motivar ajustes no planejamento, desde que respeitadas as regras de controle de escopo definidas no `docs/documents/tap/doc-tap-02-gerenciamento-escopo.md`.

## 8. Integração com os documentos do projeto

Este anexo integra-se diretamente a:

- `docs/documents/tap/doc-tap-02-gerenciamento-escopo.md`
- `docs/documents/tap/doc-tap-06-cronograma-marcos.md`
- `docs/documents/charter/doc-charter-01-termo-abertura-projeto.md`

Servindo como base formal para antecipação, mitigação e controle dos riscos do Projeto FokusLead.


