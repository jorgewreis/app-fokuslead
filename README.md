<h1><span style="color:#0b7285">:rocket: FokusLead</span></h1>

Plataforma de gestão comercial e relacionamento para times de vendas do mercado imobiliário. Este README é um resumo público para marketing, vendas e parceiros de serviços que desejam entender rapidamente o produto e sua base técnica.

Aqui você encontra uma visão de produto orientada a negócio, com narrativa clara do valor entregue e do que existe por trás da solução. A ideia é dar contexto para conversas comerciais, apresentações e processos de parceria.

> **Destaque:** foco em velocidade comercial, rastreabilidade e integração com canais sociais.

<h2><span style="color:#2f9e44">:sparkles: Principais funções</span></h2>

A FokusLead organiza o ciclo completo de vendas: da captura do lead ao fechamento, com histórico completo de contatos e visibilidade do funil por responsável e etapa. O foco está em reduzir perda de informação, padronizar a rotina do time e acelerar a resposta ao lead no momento certo.

O sistema foi pensado para times enxutos ou em crescimento, oferecendo visão do desempenho por etapa e clareza de prioridade diária. Isso permite que a gestão identifique gargalos e ajuste o processo sem depender de planilhas paralelas.

- Gestão de leads, clientes, imóveis e empreendimentos com filtros e status.
  Esse módulo centraliza os cadastros e permite segmentar por origem, interesse, faixa de preço e status, mantendo visão única por pessoa e oportunidade.
- Funil de vendas com etapas configuráveis e atribuição de responsável.
  O funil pode ser adaptado a cada operação, com regras de passagem entre etapas e indicadores de conversão por corretor.
- Histórico de interações (ligações, WhatsApp, e-mails) e anexos.
  Cada contato fica registrado com data, canal e resultado, permitindo rastrear o relacionamento e dar continuidade em qualquer troca de responsável.
- Integrações com canais externos (WhatsApp e Instagram).
  As integrações capturam conversas e leads automaticamente, reduzindo trabalho manual e acelerando o primeiro contato.
- Auditoria de ações críticas para compliance e segurança.
  Mudanças sensíveis ficam registradas com usuário e horário, ajudando em auditorias internas e exigências de governança.

**Exemplo de uso:** um lead chega via Instagram, o sistema cria o registro, atribui um corretor, registra o primeiro contato e move o lead para a etapa "Qualificação". A partir dali, o time acompanha SLA de retorno e a evolução do histórico até o fechamento.

<h2><span style="color:#845ef7">:gear: Ferramentas e tecnologias</span></h2>

Stack pensada para velocidade de entrega e escala futura, com separação clara de responsabilidades e facilidade de evolução. A base técnica prioriza estabilidade e previsibilidade para times que precisam evoluir com segurança e sem retrabalho.

O desenho de arquitetura favorece manutenção simples no início e permite abrir novos módulos no futuro, incluindo integrações e serviços especializados. Isso garante uma linha de evolução controlada conforme o produto amadurece.

- Backend: Node.js + NestJS com arquitetura limpa.
  Entrega APIs organizadas por casos de uso e domínio, facilitando testes e evolução sem impacto cruzado.
- Frontend: Next.js com SSR para páginas rápidas e indexáveis.
  Garante carregamento rápido e melhor visibilidade em buscas, com boa experiência em dispositivos móveis.
- Dados: MySQL (principal) + Redis (cache/logs).
  Combina consistência transacional com desempenho em consultas frequentes e armazenamento temporário de eventos.
- Infra: AWS (ECS Fargate, RDS, ALB, S3/CloudFront), Docker.
  Permite escalar por demanda e manter custos previsíveis, com deploys repetíveis e seguros.
- CI/CD e observabilidade: GitHub Actions + CloudWatch.
  Automatiza build e entrega e centraliza logs e métricas para detectar problemas rapidamente.

**Exemplo de uso:** páginas públicas do produto renderizam via SSR, enquanto o backend atende as operações do funil em APIs protegidas por JWT. O time de engenharia consegue entregar features sem afetar a performance do front.

<h2><span style="color:#f08c00">:briefcase: Descrição de serviços</span></h2>

Serviço orientado a times de vendas que precisam de previsibilidade, ritmo de follow-up e controle de qualidade de atendimento. A proposta é aumentar conversão com disciplina comercial e informação centralizada.

Para o gestor, o sistema se torna uma fonte confiável de indicadores, com visão por equipe, corretor e etapa. Para o vendedor, o ganho é um fluxo claro de trabalho que evita retrabalho e esquecimento de contatos importantes.

- Centralização do relacionamento com leads e clientes.
  Unifica informações de contato, preferências e etapas, evitando perda de contexto entre atendimentos.
- Organização do pipeline de vendas com visibilidade por etapa.
  Mostra volume e conversão por fase, ajudando a planejar campanhas e metas.
- Registro completo de contatos e histórico por usuário.
  Garante rastreio de atendimentos e qualidade do relacionamento, inclusive para treinamentos.
- Integração com plataformas sociais para captura e resposta rápida.
  Encaminha mensagens e leads diretamente ao time, com notificações e prioridade definida.
- Segurança e rastreabilidade para operação profissional.
  Reduz risco operacional e aumenta confiança dos clientes com controles e trilha de auditoria.

**Exemplo de uso:** o gestor acompanha conversão por etapa, identifica gargalos e padroniza o atendimento da equipe. Com isso, consegue orientar ajustes de pitch e priorizar leads com maior propensão de fechamento.

<h2><span style="color:#1c7ed6">:file_cabinet: Arquitetura de dados</span></h2>

Modelo pensado para integridade, rastreabilidade e auditoria, com histórico completo das mudanças mais relevantes. A estrutura garante consistência entre clientes, imóveis, leads e oportunidades.

O objetivo é manter um registro confiável de cada evento importante no ciclo comercial, preservando o que aconteceu e quem realizou a ação. Isso facilita auditoria, suporte e conformidade.

- Modelo relacional normalizado com chaves estrangeiras.
  Mantém consistência entre entidades e previne registros órfãos em integrações e relatórios.
- Soft delete para manter rastreabilidade de registros.
  Permite recuperar informações e entender históricos sem apagar dados de forma permanente.
- Histórico e auditoria para mudanças relevantes.
  Registra o antes e depois de campos críticos, com usuário e data.
- Retenção: logs operacionais (30 dias) e auditoria (6 meses).
  Define janela de consulta adequada para suporte e compliance, com equilíbrio de custo.

**Exemplo de uso:** um lead excluído fica como inativo e a auditoria preserva quem fez a ação e quando. Assim, a equipe consegue recuperar contexto sem perder a trilha histórica.

<h2><span style="color:#5c940d">:handshake: Para parceiros de serviços</span></h2>

Pensado para integrações e parcerias técnicas com pouco atrito e visão clara do escopo. A solução foi desenhada para permitir novos canais, conectores e automações conforme a operação exige.

Parceiros conseguem entender rapidamente onde conectar e como capturar eventos de negócio. Isso reduz tempo de onboarding e aumenta a chance de sucesso em projetos conjuntos.

- Integrações via APIs externas e webhooks.
  Parceiros podem receber eventos em tempo real e enviar dados sem depender de acesso direto ao banco.
- Camadas bem definidas para evolução e novas integrações.
  A separação de domínio e infraestrutura reduz impactos e acelera a entrega de conectores.
- Processo de homologação e compliance com políticas das plataformas.
  Garante que cada integração siga requisitos de segurança e termos das plataformas.

**Exemplo de uso:** um parceiro cria um conector para receber webhooks de leads e sincronizar com seu CRM. O fluxo permite disparar automações sem alterar o core do produto.
