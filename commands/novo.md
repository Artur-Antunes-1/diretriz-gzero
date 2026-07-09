---
description: Cria um projeto novo pela Diretriz GZero nesta pasta e inicia a Fase 1 (Ideação)
argument-hint: [descreva a ideia em 2 a 5 frases]
---

Você vai iniciar um projeto novo pela **Diretriz GZero de Projetos**.

## Passo 1 — Instalar o template nesta pasta

Localize a pasta do plugin da Diretriz (a raiz do plugin, onde vivem `template/`
e `design-system-gzero/`):
- Primeiro tente a variável de ambiente `CLAUDE_PLUGIN_ROOT`.
- Se não existir, procure em `~/.claude/plugins/marketplaces/diretriz-gzero/`.

Copie TODO o conteúdo de `<raiz-do-plugin>/template/` para a pasta atual —
incluindo o `CLAUDE.md` e as pastas ocultas `.projeto` e `.claude` — **sem
sobrescrever nenhum arquivo que já exista aqui**. Depois leia o `CLAUDE.md`
copiado por inteiro: ele é a metodologia deste projeto a partir de agora.

## Passo 2 — Iniciar a Fase 1 (Ideação)

Siga o CLAUDE.md à risca: Preparação do repositório (`.gitignore` → `git init`
→ primeiro commit → repositório privado no GitHub), depois a entrevista de
ideação, um tema por vez, sempre com 2–4 opções e recomendação marcada.

No tema da **direção visual**, ofereça também a opção "visual GZero oficial":
o pacote `<raiz-do-plugin>/design-system-gzero/` contém os tokens, fontes e
regras do Design System da casa — use-o para gerar uma das direções em HTML.
**É sugestão, nunca obrigação**: o dono do projeto escolhe livremente.

A ideia do projeto, nas palavras do dono:

$ARGUMENTS

Se os argumentos acima estiverem vazios, comece perguntando a ideia em 1
pergunta simples antes de tudo.
