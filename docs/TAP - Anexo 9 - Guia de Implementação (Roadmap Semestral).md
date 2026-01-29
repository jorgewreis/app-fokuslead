# TAP - Anexo 9: Guia de Implementação (Roadmap Semestral)

## Metadados

- **Projeto:** FokusLead
- **Documento:** TAP - Anexo 9: Guia de Implementação (Roadmap Semestral)
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
- `TAP - Anexo 8 - Guia de Funcionalidades.md`
- `TAP - Anexo 10 - Modelo Comercial e Planos de Assinatura.md`
- `TAP - Anexo 11 - Documento de Requisitos de Software (DRS).md`
- `Termo de Abertura de Projeto.md`

## 1. Visão geral

O roadmap semestral define a evolução do FokusLead em cinco módulos sequenciais, cada um com duração de 6 meses, assegurando estabilidade funcional antes da expansão de capacidades.

## 2. Módulo 1 - Base Imobiliária Estrutural

- **Período:** 0-6 meses
- **Objetivo:** Organizar dados e padronizar o portfólio
- **Posicionamento:** Sistema imobiliário profissional (sem CRM ainda)

### Funcionalidades

#### Cadastros fundamentais

- Construtoras
- Incorporadoras
- Empreendimentos
- Imóveis
- Tipos de imóveis
- Cidades
- Bairros
- Clientes (cadastro manual)
- Perfis de clientes (básicos)

#### Regras de vínculo

- Empreendimentos x construtoras (obrigatório)
- Imóveis x empreendimentos
  - Apartamentos: obrigatório
  - Casas / salas comerciais: opcional
- Bairros x cidades (obrigatório)

#### Operacional

- CRUD completo de todos os cadastros
- Interface web responsiva
- Organização e consulta do portfólio
- Controle básico de status do imóvel

### Disponibilização por plataforma

- Web Desktop (principal)
- Web Mobile (não disponível)
- iOS (não disponível)
- Android (não disponível)

### Resultado do módulo

- Base de dados sólida
- Portfólio organizado
- Preparação técnica para CRM

## 3. Módulo 2 - Entrada no CRM (Leads e integrações iniciais)

- **Período:** 7-12 meses
- **Objetivo:** Captar leads e centralizar atendimentos
- **Posicionamento:** CRM imobiliário inicial

### Funcionalidades

#### Gestão de leads

- Entidade Lead criada
- Criação automática de clientes a partir de leads
- Origem do lead (WhatsApp / Instagram)
- Data e hora de entrada
- Status inicial do lead

#### Integrações

- WhatsApp (API oficial)
  - Captação de mensagens
  - Associação automática ao cliente
- Instagram (API oficial)
  - Captação de leads e mensagens

#### Histórico

- Linha do tempo por cliente
- Registro de conversas
- Observações manuais do corretor

### Disponibilização por plataforma

- Web Desktop
- Web Mobile (layout responsivo)
- iOS (não disponível)
- Android (não disponível)

### Resultado do módulo

- Centralização dos contatos
- Redução de perda de leads
- Início do valor real de CRM

## 4. Módulo 3 - Funil de Vendas e Organização Comercial

- **Período:** 13-18 meses
- **Objetivo:** Controlar oportunidades e aumentar conversão
- **Posicionamento:** CRM funcional orientado a vendas

### Funcionalidades

#### Funil de vendas

- Etapas configuráveis:
  - Novo
  - Em atendimento
  - Visita agendada
  - Proposta enviada
  - Fechado
  - Perdido
- Movimentação visual entre etapas
- Visualização do pipeline

#### Classificação avançada

- Tags livres para clientes e leads
- Prioridade (quente, morno, frio)
- Perfil financeiro
- Intenção de compra

#### Relacionamentos

- Cliente x múltiplos imóveis
- Imóvel x múltiplos clientes
- Histórico de interesse preservado

### Disponibilização por plataforma

- Web Desktop
- Web Mobile
- PWA (progressivo)
- iOS (não disponível)
- Android (não disponível)

### Resultado do módulo

- Visão clara do processo de venda
- Menos improviso comercial
- Aumento de previsibilidade

## 5. Módulo 4 - Inteligência Operacional e Follow-up

- **Período:** 19-24 meses
- **Objetivo:** Evitar perdas por esquecimento e melhorar produtividade
- **Posicionamento:** CRM maduro para corretor profissional

### Funcionalidades

#### Agenda comercial

- Agendamento de visitas
- Lembretes de retorno
- Controle de follow-ups pendentes

#### Matching cliente x imóvel

- Cruzamento por:
  - Perfil do cliente
  - Faixa de preço
  - Tipo de imóvel
  - Localização
- Sugestão de imóveis compatíveis

#### Indicadores básicos

- Leads recebidos
- Leads atendidos
- Leads convertidos
- Tempo médio de resposta

### Disponibilização por plataforma

- Web Desktop
- Web Mobile
- PWA
- iOS (versão inicial)
- Android (versão inicial)

### Resultado do módulo

- Menos vendas perdidas
- Mais foco no que gera resultado
- Eficiência operacional visível

## 6. Módulo 5 - Consolidação, Gestão e Escala

- **Período:** 25-30 meses
- **Objetivo:** Preparar o produto para equipes e crescimento
- **Posicionamento:** Base para FokusLead Team

### Funcionalidades

#### Gestão de portfólio comercial

- Controle refinado de status de imóveis
- Destaques comerciais
- Relatórios simples de estoque

#### Visão gerencial

- Dashboard consolidado
- Indicadores comparativos
- Base para múltiplos usuários (futuro)

#### Segurança e LGPD avançada

- Logs de acesso
- Controle de visibilidade
- Anonimização estruturada
- Auditoria básica

### Disponibilização por plataforma

- Web Desktop
- Web Mobile
- PWA
- iOS (completo)
- Android (completo)

### Resultado do módulo

- Produto completo
- Preparado para equipes
- Pronto para escala comercial

## 7. Visão final do produto (30 meses)

- Módulo 1: Sistema imobiliário
- Módulo 2: CRM inicial
- Módulo 3: CRM de vendas
- Módulo 4: CRM orientado à produtividade
- Módulo 5: Plataforma escalável
