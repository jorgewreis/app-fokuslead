# TAP - Anexo 4: Gerenciamento de Custos

## Metadados

- **Projeto:** FokusLead
- **Documento:** TAP - Anexo 4: Gerenciamento de Custos
- **Versão:** 1.01
- **Responsável:** Jorge Reis
- **Data:** Atual

## Documentos relacionados

- `docs/documents/tap/doc-tap-01-stakeholders.md`
- `docs/documents/tap/doc-tap-02-gerenciamento-escopo.md`
- `docs/documents/tap/doc-tap-03-gerenciamento-riscos.md`
- `docs/documents/tap/doc-tap-05-gerenciamento-qualidade.md`
- `docs/documents/tap/doc-tap-06-cronograma-marcos.md`
- `docs/documents/tap/doc-tap-07-estrutura-analitica-projeto-eap.md`
- `docs/documents/tap/doc-tap-08-guia-funcionalidades.md`
- `docs/documents/tap/doc-tap-09-guia-implementacao-roadmap-semestral.md`
- `docs/documents/tap/doc-tap-10-modelo-comercial-planos-assinatura.md`
- `docs/documents/tap/doc-tap-11-documento-requisitos-software-drs.md`
- `docs/documents/charter/doc-charter-01-termo-abertura-projeto.md`

## 1. Introdução e objetivo

Este documento estabelece o Gerenciamento de Custos do Projeto FokusLead, definindo critérios de estimativa, composição do orçamento, reservas financeiras e mecanismos de controle ao longo de todo o programa (30 meses). O objetivo é assegurar que o projeto seja executado dentro de limites financeiros previsíveis, sustentáveis e compatíveis com o escopo, o cronograma e os riscos previamente definidos.

Este anexo complementa o `docs/documents/charter/doc-charter-01-termo-abertura-projeto.md` e os anexos de escopo, cronograma, riscos e qualidade, formando a base integrada de planejamento e controle financeiro do projeto.

## 2. Metodologia de estimativa de custos

### 2.1 Método adotado

O projeto adota como método principal de estimativa de custos a abordagem bottom-up, na qual os custos são estimados a partir das fases e pacotes de trabalho definidos na Estrutura Analítica do Projeto (EAP). Como validação complementar, utiliza-se referência top-down, comparando o orçamento consolidado com parâmetros usuais de projetos similares em complexidade e esforço.

### 2.2 Unidade de custo

A unidade base de custo do projeto é a hora técnica, considerando o custo total de esforço, incluindo:

- Desenvolvimento
- Infraestrutura básica
- Ferramentas
- Custos operacionais associados

**Valor adotado:** R$ 150,00 por hora

### 2.3 Capacidade de trabalho

Para fins de planejamento financeiro, considera-se uma capacidade média de:

- 10 horas semanais de dedicação ao projeto

Premissa oficial:

- 1 semana de projeto = 10 horas = R$ 1.500,00

## 3. Classificação dos custos

O orçamento do projeto contempla as seguintes categorias:

- **Custos diretos:** serviços e recursos aplicados diretamente ao produto.
- **Custos fixos:** licenças, ferramentas e serviços recorrentes.
- **Custos variáveis:** APIs, serviços sob demanda e consumo por volume.

Os custos indiretos são absorvidos no valor da hora técnica e não são discriminados separadamente.

## 4. Orçamento do projeto

### 4.1 Custo por módulo (referência)

Premissa: 6 meses por módulo, com aproximadamente 26 semanas.

| Módulo | Período | Horas estimadas | Custo estimado |
| --- | --- | --- | --- |
| Módulo 1 - Base Imobiliária | 0-6 meses | 260 h | R$ 39.000,00 |
| Módulo 2 - CRM inicial | 7-12 meses | 260 h | R$ 39.000,00 |
| Módulo 3 - CRM de vendas | 13-18 meses | 260 h | R$ 39.000,00 |
| Módulo 4 - Produtividade | 19-24 meses | 260 h | R$ 39.000,00 |
| Módulo 5 - Escala e Team | 25-30 meses | 260 h | R$ 39.000,00 |
| **Total** | **30 meses** | **1.300 h** | **R$ 195.000,00** |

### 4.2 Reservas financeiras

#### Reserva de contingência

Destinada à cobertura de riscos identificados no `docs/documents/tap/doc-tap-03-gerenciamento-riscos.md` (APIs, performance, autenticação, estabilidade, LGPD).

- Percentual adotado: 10%
- Valor estimado: R$ 19.500,00

### 4.3 Orçamento total do programa

- **Orçamento total estimado:** R$ 214.500,00

Os valores são referências iniciais e devem ser revisados a cada módulo, considerando variações de esforço, complexidade e disponibilidade.

### 4.4 Custos variáveis (controle contínuo)

Os custos variáveis serão monitorados mensalmente, com foco em:

- Consumo de APIs externas (WhatsApp e Instagram)
- Infraestrutura (banco de dados, storage e tráfego)
- Serviços de monitoramento e observabilidade

## 5. Controle de custos

O controle de custos será realizado de forma contínua durante a execução do projeto, observando:

- Aderência ao cronograma definido no `docs/documents/tap/doc-tap-06-cronograma-marcos.md`
- Consumo real de tempo por fase
- Impacto de atrasos ou ajustes no custo implícito do esforço

Desvios relevantes poderão exigir:

- Uso da reserva de contingência
- Repriorização de entregas
- Replanejamento de esforço por módulo

## 6. Integração com os documentos do projeto

Este anexo integra-se diretamente a:

- `docs/documents/tap/doc-tap-02-gerenciamento-escopo.md`
- `docs/documents/tap/doc-tap-03-gerenciamento-riscos.md`
- `docs/documents/tap/doc-tap-06-cronograma-marcos.md`
- `docs/documents/charter/doc-charter-01-termo-abertura-projeto.md`

Servindo como referência formal para planejamento, monitoramento e tomada de decisão financeira do Projeto FokusLead.


