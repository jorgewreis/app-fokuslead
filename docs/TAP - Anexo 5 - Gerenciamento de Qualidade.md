# TAP - Anexo 5: Gerenciamento de Qualidade

## Metadados

- **Projeto:** FokusLead
- **Documento:** TAP - Anexo 5: Gerenciamento de Qualidade
- **Versão:** 1.01
- **Responsável:** Jorge Reis
- **Data:** Atual

## Documentos relacionados

- `TAP - Anexo 1 - Stakeholders.md`
- `TAP - Anexo 2 - Gerenciamento de Escopo.md`
- `TAP - Anexo 3 - Gerenciamento de Riscos.md`
- `TAP - Anexo 4 - Gerenciamento de Custos.md`
- `TAP - Anexo 6 - Cronograma e Marcos.md`
- `TAP - Anexo 7 - Estrutura Analítica do Projeto (EAP).md`
- `TAP - Anexo 8 - Guia de Funcionalidades.md`
- `TAP - Anexo 9 - Guia de Implementação (Roadmap Semestral).md`
- `TAP - Anexo 10 - Modelo Comercial e Planos de Assinatura.md`
- `TAP - Anexo 11 - Documento de Requisitos de Software (DRS).md`
- `Termo de Abertura de Projeto.md`

## 1. Introdução e objetivo

Este documento estabelece o Gerenciamento da Qualidade do Projeto FokusLead, definindo critérios, práticas, responsabilidades e mecanismos de controle necessários para assegurar que o produto, em sua visão completa, atenda aos padrões de qualidade esperados para uso comercial contínuo.

O objetivo do gerenciamento da qualidade é garantir que o produto entregue:

- Atenda aos requisitos funcionais definidos
- Ofereça boa experiência de uso
- Seja estável, seguro e sustentável do ponto de vista técnico

## 2. Conceito de qualidade adotado

A qualidade do FokusLead é definida como o equilíbrio entre conformidade técnica e experiência do usuário, com prioridade para a fluidez dos fluxos críticos do CRM imobiliário. O foco é assegurar que o produto seja utilizável diariamente, com baixa fricção operacional, mantendo segurança e integridade de dados.

## 3. Referências e abordagem de qualidade

O gerenciamento da qualidade adota uma abordagem híbrida, baseada em:

- Boas práticas de produtos digitais (usabilidade, performance, estabilidade)
- Referências conceituais do PMBOK e padrões de qualidade (aplicados de forma objetiva)

A garantia da qualidade ocorre por meio de:

- Validação contínua durante o desenvolvimento
- Checkpoints formais ao final de cada bloco funcional e módulo do projeto

## 4. Dimensões de qualidade monitoradas

As seguintes dimensões de qualidade são monitoradas ao longo de todo o projeto:

- Funcionalidade: aderência aos requisitos definidos
- Usabilidade: clareza, facilidade de uso e fluidez dos fluxos
- Performance: tempo de resposta e carregamento
- Estabilidade: ausência de erros críticos e travamentos
- Segurança e LGPD: proteção de dados e controle de acesso
- Manutenibilidade: organização do código e facilidade de evolução
- Escalabilidade: capacidade de crescimento de base e usuários

## 5. Critério geral de qualidade

O produto será considerado com qualidade aceitável quando:

- Os fluxos principais do sistema funcionarem sem fricção relevante
- Os dados permanecerem íntegros e rastreáveis
- O desempenho suportar o volume esperado do módulo vigente

Falhas críticas que impeçam o uso normal ou comprometam a segurança não são aceitáveis.

## 6. Fluxos críticos para aceitação da qualidade

Os seguintes fluxos são considerados críticos e devem obrigatoriamente funcionar de forma fluida:

- Login e controle de sessão
- Cadastro e edição de clientes
- Cadastro e edição de imóveis
- Relacionamento cliente x imóvel
- Uso de perfis, tags e filtros
- Navegação geral (menus, listagens e retornos)
- Registro de leads e origem
- Funil de vendas e movimentação de oportunidades
- Agenda e follow-ups

## 7. Tipos de testes adotados

Para validação da qualidade, serão adotados os seguintes tipos de teste:

- Testes funcionais manuais
- Testes de usabilidade (uso real e análise de fricção)
- Testes de performance (tempo de carregamento)
- Testes de estabilidade (uso contínuo e verificação de erros)
- Testes básicos de segurança (controle de acesso e exposição de dados)
- Testes de integração com APIs externas

## 8. Frequência e momento dos testes

Durante cada módulo semestral, os testes de qualidade serão realizados:

- Ao final de cada bloco funcional, conforme definido no `TAP - Anexo 6 - Cronograma e Marcos.md`
- Em validações formais ao final de cada módulo

## 9. Responsabilidade pela qualidade

O responsável final pela validação da qualidade é o responsável técnico e de produto do projeto, que realizará:

- Validação funcional
- Verificação dos critérios de qualidade
- Aprovação formal por meio de checklist documentado

## 10. Checklist de qualidade

A validação da qualidade será realizada por meio de um checklist simples, com itens avaliados como:

- OK
- Não OK

O checklist será utilizado para:

- Blocos funcionais
- Encerramento de módulos
- Aceitação final do produto

## 11. Tratamento de não conformidades

Quando um bloco funcional ou módulo não atender aos critérios de qualidade, aplica-se a seguinte regra:

- A correção da não conformidade é obrigatória antes do avanço para o próximo bloco ou módulo.

Não é permitido avançar no cronograma mantendo falhas relevantes nos fluxos críticos.

## 12. Integração com os documentos do projeto

Este anexo integra-se diretamente a:

- `TAP - Anexo 2 - Gerenciamento de Escopo.md`
- `TAP - Anexo 3 - Gerenciamento de Riscos.md`
- `TAP - Anexo 4 - Gerenciamento de Custos.md`
- `TAP - Anexo 6 - Cronograma e Marcos.md`
- `Termo de Abertura de Projeto.md`

Servindo como referência oficial para planejamento, execução, validação e aceitação da qualidade do Projeto FokusLead.
