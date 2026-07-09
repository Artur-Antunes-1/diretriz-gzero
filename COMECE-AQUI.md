# Comece aqui — Diretriz GZero para colegas

> Você imagina. A IA constrói. Nada se perde.
> Para entender o que é isso em 5 minutos, abra o site:
> **https://artur-antunes-1.github.io/diretriz-gzero/**
> (o site é público; este repositório é privado)

A Diretriz GZero é a metodologia da casa para criar projetos com o Claude Code:
você conversa e decide o produto; a IA desenvolve tudo sozinha, com qualidade
verificada e sem perder nada entre sessões. **Não precisa saber programar.**

## O que você precisa (uma vez só)

1. **Claude Code** instalado e logado.
2. **GitHub**: uma conta com acesso a este repositório, e o GitHub CLI logado —
   instale em https://cli.github.com e rode `gh auth login` num terminal.
   (É o que permite à IA guardar seus projetos num cofre privado na nuvem.)

## Instalar a Diretriz (o jeito recomendado: plugin)

Dentro do Claude Code, rode uma vez:

```
/plugin marketplace add Artur-Antunes-1/diretriz-gzero
/plugin install diretriz@diretriz-gzero
```

(Precisa de acesso ao repositório — peça o convite ao Artur — e do git/gh
logado na sua conta.)

Pronto. Em qualquer pasta, para sempre:

| Situação | Comando |
|---|---|
| Criar um projeto novo | `/diretriz:novo minha ideia em 2–5 frases` |
| Adotar num projeto que já existe | `/diretriz:adotar` |
| Atualizar um projeto para a versão nova | `/diretriz:atualizar` |
| Continuar qualquer projeto, em qualquer dia | digite apenas `continuar` |

## Sem plugin (alternativas)

- **Clonar o repo:** `git clone https://github.com/Artur-Antunes-1/diretriz-gzero.git`
  e usar os prompts prontos do `COMO-INICIAR.md` (ajuste o caminho do template
  para onde você clonou).
- **Só o prompt:** copie o prompt de "Projeto novo" do `COMO-INICIAR.md`,
  troque o caminho do template pela URL deste repositório e peça ao Claude para
  clonar e copiar. Ele faz sozinho.

## O que esperar

- **Fase 1 — Ideação:** a IA te entrevista (30–50 min), sempre com opções
  prontas, e gera 2–3 propostas visuais em HTML para você escolher olhando.
  Uma delas pode ser no **Design System GZero** (o visual da casa) — é sugestão,
  não obrigação.
- **Fase 2 — Travamento:** você bate o martelo numa lista de decisões. Depois
  disso a IA nunca mais pergunta essas coisas.
- **Fase 3 — Execução:** a IA trabalha sozinha, meta a meta, testando e
  revisando tudo. A cada marco, deixa screenshots para você espiar. Quando uma
  sessão enche, ela pede: *"abra uma nova sessão e diga: continuar"*.
- **Fase 4 — Entrega:** ela testa os critérios de sucesso na prática, demonstra
  e publica do jeito combinado.

Seu papel operacional depois do travamento é literalmente **uma palavra**:
`continuar`.

## Regras da casa (as inegociáveis)

1. Você decide **o quê**; a IA decide **o como**.
2. Decisão travada não se reabre (só você destrava, por escrito).
3. Nada é "pronto" sem funcionar de verdade, revisado por outros agentes.
4. Tudo fica anotado em arquivos e guardado num repositório **privado** no
   GitHub — nunca dependa da memória da conversa.
5. A IA só te interrompe para: dinheiro, contas externas, publicação, ou algo
   que contrarie o combinado.

Dúvidas sobre o funcionamento por dentro: leia o `README.md` e o
`template/CLAUDE.md` (a metodologia completa que a IA segue).

*com amor & spray rosa — somos gzero* ★
