# Tipos de commit e quando usar

Este guia descreve os tipos de commit mais comuns para manter o historico do repositorio claro e consistente. Use o prefixo apropriado no inicio da mensagem de commit.

## Tipos

- feat: nova funcionalidade ou incremento de comportamento que o usuario percebe.
- fix: correcao de bug ou ajuste que resolve um problema existente.
- refactor: mudanca interna de codigo sem alterar comportamento externo (ex.: reorganizar funcoes, remover duplicacao).
- docs: alteracoes apenas em documentacao (README, guias, comentarios relevantes).
- style: ajustes de formatacao ou estilo de codigo sem impacto logico (ex.: espacos, lint, ordem de imports).
- perf: melhorias de desempenho sem mudar comportamento externo (ex.: otimizacao de consultas).
- test: adicao ou ajuste de testes sem mudar codigo de producao.
- chore: tarefas de manutencao que nao afetam o codigo de producao nem testes diretamente (ex.: configs, deps, scripts).
- build: alteracoes no build ou empacotamento (ex.: bundlers, scripts de build).
- ci: alteracoes em pipelines e automacoes de CI (ex.: GitHub Actions).
- revert: desfaz um commit anterior de forma explicita.
- deps: atualizacoes de dependencias sem mudanca de comportamento (ex.: bump de versao).
- config: ajustes de configuracao de ambiente ou ferramentas (ex.: ESLint, Prettier).
- release: preparacao de versao (ex.: changelog, tags, versionamento).
- i18n: ajustes de internacionalizacao e traducao.
- ux: melhorias de experiencia de uso sem nova funcionalidade principal.

## Dicas rapidas

- Seja objetivo: "feat: adicionar filtro por data na lista".
- Se houver mais de uma mudanca, priorize o tipo com maior impacto.
- Evite misturar multiplos tipos no mesmo commit; se possivel, separe.

## Modelo padrao de commit

Formato:

`tipo: descricao do commit`

## Exemplos

- `docs: novo documento criado`
- `feat: permitir exportar relatorio em CSV`
- `fix: corrigir erro ao salvar formulario`
- `refactor: separar validacoes em modulo`
- `style: ordenar imports no controller`
- `perf: reduzir consultas no carregamento`
- `test: adicionar testes para login`
- `chore: atualizar versao do Node`
- `build: ajustar script de build para producao`
- `ci: adicionar job de lint no pipeline`
- `revert: desfazer commit que quebrou deploy`
- `deps: atualizar react para 18.3`
- `config: ajustar regras do eslint`
- `release: preparar versao 1.4.0`
- `i18n: traduzir mensagens de erro`
- `ux: melhorar fluxo de cadastro em 2 passos`
