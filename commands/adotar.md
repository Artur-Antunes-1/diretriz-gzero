---
description: Adota a Diretriz GZero num projeto que JÁ existe nesta pasta (ideação reversa, sem perder nada)
---

Você vai adotar a **Diretriz GZero de Projetos** neste projeto existente.

## Passo 1 — Instalar o template sem sobrescrever

Localize a pasta do plugin (via `CLAUDE_PLUGIN_ROOT` ou
`~/.claude/plugins/marketplaces/diretriz-gzero/`). Copie o conteúdo de
`<raiz-do-plugin>/template/` para esta pasta — incluindo `.projeto` e `.claude`
— **sem sobrescrever nada que já exista**. Se já existir um `CLAUDE.md`, mescle:
as regras da Diretriz entram primeiro e o conteúdo antigo vira uma seção
"Notas específicas do projeto" no fim. Leia o `CLAUDE.md` resultante.

## Passo 2 — Adoção (ideação reversa)

1. Estude o projeto como ele está (código, README, git log se houver) e diga ao
   dono, em 5 linhas, o que você entendeu que ele é.
2. Preencha pelo que leu: `VISAO.md` (o que o projeto é), `PADROES.md` (a stack
   e as convenções REAIS do código), `ESTADO.md` (onde está agora, como rodar) e
   `ROADMAP.md` — o que já funciona vira metas ✅ de um "Marco 0 — herdado";
   o que está pela metade ou faltando vira metas ⬜.
3. Só pergunte o que NÃO dá para inferir do código (público, escopo, aparência
   desejada, o que fica de fora) — com opções prontas, como na Fase 1. Se o
   projeto tem interface e o dono gosta do visual atual, o visual atual vira a
   referência travada; se quiser mudar, gere direções em HTML (o pacote
   `design-system-gzero/` do plugin é uma das opções — sugestão, não obrigação).
4. Registre em `DECISOES.md`: escolhas já feitas no projeto como TRAVADAS
   (são história, não se reabrem sem pedido) e as que dependem do dono como
   PENDENTES.
5. Cumpra a Preparação do repositório do CLAUDE.md (`.gitignore` com proteção
   de `.env`, git, repositório privado no GitHub) se ainda não existir.
6. Siga para a Fase 2 (travamento) e, dali em diante, a Diretriz vale
   integralmente.
