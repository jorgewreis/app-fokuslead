<h1><span style="color:#0b7285">:rocket: FokusLead</span></h1>

Plataforma de gestao comercial e relacionamento para times de vendas do mercado imobiliario. Este README e um resumo publico para marketing, vendas e parceiros de servicos que desejam entender rapidamente o produto e sua base tecnica.

Aqui voce encontra uma visao de produto orientada a negocio, com narrativa clara do valor entregue e do que existe por tras da solucao. A ideia e dar contexto para conversas comerciais, apresentacoes e processos de parceria.

> **Destaque:** foco em velocidade comercial, rastreabilidade e integracao com canais sociais.

<h2><span style="color:#2f9e44">:sparkles: Principais funcoes</span></h2>

A FokusLead organiza o ciclo completo de vendas: da captura do lead ao fechamento, com historico completo de contatos e visibilidade do funil por responsavel e etapa. O foco esta em reduzir perda de informacao, padronizar a rotina do time e acelerar a resposta ao lead no momento certo.

O sistema foi pensado para times enxutos ou em crescimento, oferecendo visao do desempenho por etapa e clareza de prioridade diaria. Isso permite que a gestao identifique gargalos e ajuste o processo sem depender de planilhas paralelas.

- Gestao de leads, clientes, imoveis e empreendimentos com filtros e status.
  Esse modulo centraliza os cadastros e permite segmentar por origem, interesse, faixa de preco e status, mantendo visao unica por pessoa e oportunidade.
- Funil de vendas com etapas configuraveis e atribuicao de responsavel.
  O funil pode ser adaptado a cada operacao, com regras de passagem entre etapas e indicadores de conversao por corretor.
- Historico de interacoes (liga, WhatsApp, e-mails) e anexos.
  Cada contato fica registrado com data, canal e resultado, permitindo rastrear o relacionamento e dar continuidade em qualquer troca de responsavel.
- Integracoes com canais externos (WhatsApp e Instagram).
  As integracoes capturam conversas e leads automaticamente, reduzindo trabalho manual e acelerando o primeiro contato.
- Auditoria de acoes criticas para compliance e seguranca.
  Mudancas sensiveis ficam registradas com usuario e horario, ajudando em auditorias internas e exigencias de governanca.

**Exemplo de uso:** um lead chega via Instagram, o sistema cria o registro, atribui um corretor, registra o primeiro contato e move o lead para a etapa "Qualificacao". A partir dali, o time acompanha SLA de retorno e a evolucao do historico ate o fechamento.

<h2><span style="color:#845ef7">:gear: Ferramentas e tecnologias</span></h2>

Stack pensada para velocidade de entrega e escala futura, com separacao clara de responsabilidades e facilidade de evolucao. A base tecnica prioriza estabilidade e previsibilidade para times que precisam evoluir com seguranca e sem retrabalho.

O desenho de arquitetura favorece manutencao simples no inicio e permite abrir novos modulos no futuro, incluindo integracoes e servicos especializados. Isso garante uma linha de evolucao controlada conforme o produto amadurece.

- Backend: Node.js + NestJS com arquitetura limpa.
  Entrega APIs organizadas por casos de uso e dominio, facilitando testes e evolucao sem impacto cruzado.
- Frontend: Next.js com SSR para paginas rapidas e indexaveis.
  Garante carregamento rapido e melhor visibilidade em buscas, com boa experiencia em dispositivos moveis.
- Dados: MySQL (principal) + Redis (cache/logs).
  Combina consistencia transacional com desempenho em consultas frequentes e armazenamento temporario de eventos.
- Infra: AWS (ECS Fargate, RDS, ALB, S3/CloudFront), Docker.
  Permite escalar por demanda e manter custos previsiveis, com deploys repetiveis e seguros.
- CI/CD e observabilidade: GitHub Actions + CloudWatch.
  Automatiza build e entrega e centraliza logs e metricas para detectar problemas rapidamente.

**Exemplo de uso:** pages publicas do produto renderizam via SSR, enquanto o backend atende as operacoes do funil em APIs protegidas por JWT. O time de engenharia consegue entregar features sem afetar a performance do front.

<h2><span style="color:#f08c00">:briefcase: Descricao de servicos (visao comercial)</span></h2>

Servico orientado a times de vendas que precisam de previsibilidade, ritmo de follow-up e controle de qualidade de atendimento. A proposta e aumentar conversao com disciplina comercial e informacao centralizada.

Para o gestor, o sistema se torna uma fonte confiavel de indicadores, com visao por equipe, corretor e etapa. Para o vendedor, o ganho e um fluxo claro de trabalho que evita retrabalho e esquecimento de contatos importantes.

- Centralizacao do relacionamento com leads e clientes.
  Unifica informacoes de contato, preferencias e etapas, evitando perda de contexto entre atendimentos.
- Organizacao do pipeline de vendas com visibilidade por etapa.
  Mostra volume e conversao por fase, ajudando a planejar campanhas e metas.
- Registro completo de contatos e historico por usuario.
  Garante rastreio de atendimentos e qualidade do relacionamento, inclusive para treinamentos.
- Integracao com plataformas sociais para captura e resposta rapida.
  Encaminha mensagens e leads diretamente ao time, com notificacoes e prioridade definida.
- Seguranca e rastreabilidade para operacao profissional.
  Reduz risco operacional e aumenta confianca dos clientes com controles e trilha de auditoria.

**Exemplo de uso:** o gestor acompanha conversao por etapa, identifica gargalos e padroniza o atendimento da equipe. Com isso, consegue orientar ajustes de pitch e priorizar leads com maior propensao de fechamento.

<h2><span style="color:#1c7ed6">:database: Arquitetura de dados</span></h2>

Modelo pensado para integridade, rastreabilidade e auditoria, com historico completo das mudancas mais relevantes. A estrutura garante consistencia entre clientes, imoveis, leads e oportunidades.

O objetivo e manter um registro confiavel de cada evento importante no ciclo comercial, preservando o que aconteceu e quem realizou a acao. Isso facilita auditoria, suporte e conformidade.

- Modelo relacional normalizado com chaves estrangeiras.
  Mantem consistencia entre entidades e previne registros orfaos em integracoes e relatorios.
- Soft delete para manter rastreabilidade de registros.
  Permite recuperar informacoes e entender historicos sem apagar dados de forma permanente.
- Historico e auditoria para mudancas relevantes.
  Registra o antes e depois de campos criticos, com usuario e data.
- Retencao: logs operacionais (30 dias) e auditoria (6 meses).
  Define janela de consulta adequada para suporte e compliance, com equilibrio de custo.

**Exemplo de uso:** um lead excluido fica como inativo e a auditoria preserva quem fez a acao e quando. Assim, a equipe consegue recuperar contexto sem perder a trilha historica.

<h2><span style="color:#5c940d">:handshake: Para parceiros de servicos</span></h2>

Pensado para integracoes e parcerias tecnicas com pouco atrito e visao clara do escopo. A solucao foi desenhada para permitir novos canais, conectores e automacoes conforme a operacao exige.

Parceiros conseguem entender rapidamente onde conectar e como capturar eventos de negocio. Isso reduz tempo de onboarding e aumenta a chance de sucesso em projetos conjuntos.

- Integracoes via APIs externas e webhooks.
  Parceiros podem receber eventos em tempo real e enviar dados sem depender de acesso direto ao banco.
- Camadas bem definidas para evolucao e novas integracoes.
  A separacao de dominio e infraestrutura reduz impactos e acelera a entrega de conectores.
- Processo de homologacao e compliance com politicas das plataformas.
  Garante que cada integracao siga requisitos de seguranca e termos das plataformas.

**Exemplo de uso:** um parceiro cria um conector para receber webhooks de leads e sincronizar com seu CRM. O fluxo permite disparar automacoes sem alterar o core do produto.
