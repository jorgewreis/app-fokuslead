# TAP - Anexo 8: Guia de Funcionalidades

## Metadados

- **Projeto:** FokusLead
- **Documento:** TAP - Anexo 8: Guia de Funcionalidades
- **Versão:** 1.01
- **Responsável:** Jorge Reis
- **Data:** Atual

## Documentos relacionados

- `TAP - Anexo 1 - Stakeholders.md`
- `TAP - Anexo 2 - Gerenciamento de Escopo.md`
- `TAP - Anexo 3 - Gerenciamento de Riscos.md`
- `TAP - Anexo 4 - Gerenciamento de Custos.md`
- `TAP - Anexo 5 - Gerenciamento de Qualidade.md`
- `TAP - Anexo 6 - Cronograma e Marcos.md`
- `TAP - Anexo 7 - Estrutura Analítica do Projeto (EAP).md`
- `TAP - Anexo 9 - Guia de Implementação (Roadmap Semestral).md`
- `TAP - Anexo 10 - Modelo Comercial e Planos de Assinatura.md`
- `TAP - Anexo 11 - Documento de Requisitos de Software (DRS).md`
- `Termo de Abertura de Projeto.md`

## 1. Visão geral

Este guia consolida as principais funcionalidades do FokusLead na visão completa do produto, servindo como referência de escopo funcional e alinhamento entre módulos, requisitos e modelo comercial.

## 2. Núcleo do domínio

- Autenticação e controle de sessão
- Gestão de usuários (Team) e permissões
- Controle de acesso por perfil
- Logs básicos de acesso e auditoria

## 3. Estrutura imobiliária

- Cadastro de construtoras e incorporadoras
- Cadastro de empreendimentos e vínculos obrigatórios
- Cadastro de tipos de imóveis
- Cadastro de imóveis com atributos comerciais
- Cadastro de cidades e bairros com vínculos obrigatórios
- Status e disponibilidade de imóveis

## 4. Gestão comercial

- Cadastro de clientes e perfis
- Cadastro de leads (origem, data e canal)
- Conversão de lead em cliente com histórico preservado
- Linha do tempo por cliente
- Registro de interações (mensagens, notas, ligações)
- Relacionamento cliente x imóvel (N:N)

## 5. Funil de vendas e oportunidades

- Etapas configuráveis do funil
- Movimentação visual de oportunidades
- Pipeline comercial
- Classificação avançada por tags e prioridade
- Histórico de interesse por cliente e imóvel

## 6. Produtividade e agenda

- Agenda comercial integrada
- Agendamento de visitas e retornos
- Lembretes e follow-ups
- Controle de pendências

## 7. Inteligência e indicadores

- Indicadores de leads recebidos, atendidos e convertidos
- Tempo médio de resposta
- Dashboards operacionais
- Dashboards gerenciais (Team)

## 8. Integrações externas

- WhatsApp Business API
- Instagram API
- Camada de abstração para integrações
- Registro de eventos e mensagens por integração

## 9. Segurança e LGPD

- Consentimento e rastreabilidade
- Mascaramento e proteção de dados sensíveis
- Políticas de retenção e exclusão controlada
- Logs e auditoria básica

## 10. Plataformas suportadas

- Web Desktop
- Web Mobile
- PWA
- iOS (evolução gradual)
- Android (evolução gradual)

## 11. Mapeamento por módulo (resumo)

- **Módulo 1:** base imobiliária e cadastros
- **Módulo 2:** leads e integrações iniciais
- **Módulo 3:** funil de vendas e organização comercial
- **Módulo 4:** produtividade, agenda e matching
- **Módulo 5:** gestão, escala e governança

## 12. Observações finais

As funcionalidades listadas representam o escopo completo do produto. A entrega é progressiva, conforme definido no `TAP - Anexo 9 - Guia de Implementação (Roadmap Semestral).md`.
