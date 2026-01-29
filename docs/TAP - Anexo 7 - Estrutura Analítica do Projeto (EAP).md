# TAP - Anexo 7: Estrutura Analítica do Projeto (EAP)

## Metadados

- **Projeto:** FokusLead
- **Documento:** TAP - Anexo 7: Estrutura Analítica do Projeto (EAP)
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
- `TAP - Anexo 8 - Guia de Funcionalidades.md`
- `TAP - Anexo 9 - Guia de Implementação (Roadmap Semestral).md`
- `TAP - Anexo 10 - Modelo Comercial e Planos de Assinatura.md`
- `TAP - Anexo 11 - Documento de Requisitos de Software (DRS).md`
- `Termo de Abertura de Projeto.md`

## 1. Introdução

A Estrutura Analítica do Projeto (EAP), também denominada Work Breakdown Structure (WBS), representa a decomposição hierárquica de todo o trabalho necessário para a entrega completa do Programa FokusLead, abrangendo desde a construção da base imobiliária estrutural até a consolidação da plataforma como CRM imobiliário escalável, conforme definido no escopo global do projeto.

Esta EAP não se limita ao MVP, constituindo a linha de base oficial de escopo do programa, sendo o principal instrumento para:

- Planejamento e controle do cronograma semestral
- Estimativa e acompanhamento de esforço e complexidade
- Controle rigoroso de escopo e prevenção de scope creep
- Gestão de riscos técnicos e operacionais
- Validação objetiva das entregas por módulo
- Comunicação clara entre direção estratégica e execução técnica

Toda funcionalidade, integração ou evolução do produto deve estar explicitamente representada nesta estrutura.

## 2. Estrutura da EAP - visão geral

### 2.1 Nível 1 - Programa

- Programa FokusLead

### 2.2 Nível 2 - Produtos

- FokusLead One
- FokusLead Team

### 2.3 Nível 3 - Domínios funcionais globais

Aplicáveis a todo o programa, com expansão progressiva conforme o módulo:

- Interface, experiência e navegação
- Gestão de acesso, usuários e autenticação
- Cadastro e estrutura imobiliária
- Gestão de imóveis e portfólio
- Gestão de clientes e leads
- Relacionamentos comerciais cliente x imóvel
- Funil de vendas e processo comercial
- Agenda, follow-ups e produtividade
- Integrações externas (APIs)
- Indicadores, dashboards e relatórios
- Segurança da informação e LGPD
- Governança, auditoria e escalabilidade

## 3. Estrutura analítica detalhada (níveis 4 e 5)

### 3.1 Interface, experiência e navegação

#### Identidade visual e layout base

- Paleta de cores
- Tipografia institucional
- Grid, espaçamentos e padrões
- Botões, ícones e ações
- Formulários e estados visuais
- Estilos globais reutilizáveis

#### Telas de acesso e navegação inicial

- Tela de login
- Validação de campos
- Mensagens de erro e sucesso
- Redirecionamento pós-login
- Tratamento visual de sessão

#### Telas principais e dashboards

- Tela inicial
- Dashboard operacional
- Organização de widgets
- Navegação entre módulos

#### Componentes de navegação

- Menu principal
- Estados ativos
- Breadcrumbs
- Navegação contextual

#### Listagens e consultas

- Padrão de listagens
- Paginação
- Ordenação
- Ações rápidas
- Feedback de carregamento

#### Responsividade e multiplataforma

- Web Desktop
- Web Mobile
- PWA
- iOS
- Android

### 3.2 Gestão de acesso, usuários e autenticação

#### Login e sessão

- Fluxo de autenticação
- Criação e validação de sessão
- Sessão expirada

#### Gestão de credenciais

- Recuperação de senha
- Tokens temporários
- Regras de segurança

#### Segurança de acesso

- Proteção de rotas
- Limite de tentativas
- Logs de autenticação

#### Gestão de usuários (Team)

- Cadastro de usuários
- Perfis e permissões
- Hierarquia e visibilidade

### 3.3 Cadastro e estrutura imobiliária

#### Construtoras e incorporadoras

- Modelagem de dados
- Cadastro, edição e listagem
- Exclusão lógica
- Validações

#### Empreendimentos

- Vínculo obrigatório
- Cadastro e edição
- Consultas por construtora
- Regras de dependência

#### Localização

- Cidades
- Bairros
- Vínculos obrigatórios

### 3.4 Gestão de imóveis e portfólio

#### Cadastro de imóveis

- Tipos de imóveis
- Regras por categoria
- Atributos comerciais

#### Status e disponibilidade

- Disponível
- Reservado
- Vendido
- Inativo

#### Consultas e organização

- Filtros
- Busca avançada
- Destaques comerciais

### 3.5 Gestão de clientes e leads

#### Cadastro de clientes

- Cadastro manual
- Dados pessoais
- Observações

#### Gestão de leads

- Entidade Lead
- Origem do lead
- Data e canal
- Evolução para cliente

#### Histórico de interações

- Linha do tempo
- Conversas
- Anotações manuais

### 3.6 Relacionamentos cliente x imóvel

#### Interesses do cliente

- Múltiplos imóveis por cliente

#### Interessados no imóvel

- Múltiplos clientes por imóvel

#### Preservação histórica

- Regras de exclusão
- Integridade do histórico

### 3.7 Funil de vendas e processo comercial

#### Etapas do funil

- Novo
- Em atendimento
- Visita
- Proposta
- Fechado
- Perdido

#### Movimentação e pipeline

- Visualização do funil
- Alteração de etapas

### 3.8 Agenda, follow-ups e produtividade

#### Agenda comercial

- Visitas
- Compromissos

#### Follow-ups

- Lembretes
- Pendências

### 3.9 Integrações externas

- WhatsApp Business API
- Instagram API
- Camada de abstração de integrações

### 3.10 Indicadores, dashboards e relatórios

#### Indicadores operacionais

- Leads
- Conversões
- Tempo de resposta

#### Dashboards gerenciais (Team)

- Indicadores comparativos
- Consolidação por equipe

### 3.11 Segurança da informação e LGPD

- Proteção de dados
- Anonimização
- Consentimento

### 3.12 Governança, auditoria e escalabilidade

- Logs de acesso
- Auditoria básica
- Preparação para escala

## 4. Dicionário da EAP - diretrizes gerais

Para todos os pacotes de trabalho:

- **Responsável:** Jorge Reis
- **Critérios de aceitação:** funcionalidade aderente ao escopo aprovado, ausência de falhas críticas e fluxos principais operacionais
- **Estimativas:** conforme cronograma semestral oficial
- **Custos:** conforme planejamento financeiro do projeto
- **Controle:** checklist de validação e testes por módulo

## 5. Encerramento do anexo

Esta Estrutura Analítica representa a linha de base oficial do escopo do Programa FokusLead, sendo referência obrigatória para:

- Controle de mudanças
- Planejamento e execução dos ciclos semestrais
- Avaliação de riscos
- Validação das entregas

Qualquer alteração nesta EAP deverá seguir formalmente o processo de controle de mudanças definido no `TAP - Anexo 2 - Gerenciamento de Escopo.md`.
