# Prompts prontos — copie e cole

## Pré-requisito (uma vez só, para todos os projetos)

Todo projeto ganha automaticamente um repositório **privado** no GitHub, como
backup fora do computador. Para isso funcionar, o GitHub CLI precisa estar
instalado e logado na sua conta — uma única vez, para sempre:

1. Instale: https://cli.github.com (botão "Download for Windows")
2. Num terminal, rode: `gh auth login` e siga as instruções (login pelo navegador)

Se não estiver logado, nada quebra: o Claude avisa, segue trabalhando
localmente e envia tudo ao GitHub assim que você logar.

## 1. Projeto novo

Crie uma pasta nova, abra o Claude Code nela e cole isto (preenchendo a ideia no final):

```
Novo projeto pela Diretriz GZero.

Primeiro: copie TODO o conteúdo de
"C:\Users\artur\Área de Trabalho\Gzero\DiretrizDeProjetos\template"
para esta pasta — incluindo o CLAUDE.md e as pastas ocultas .projeto e .claude —
e leia o CLAUDE.md copiado.

Depois inicie a Fase 1 (Ideação). Minha ideia é:

[DESCREVA A IDEIA EM 2 A 5 FRASES — o que é, para quem, o que resolve]
```

## 1b. Projeto que JÁ EXISTE — adotar a Diretriz

Abra o Claude Code na pasta do projeto existente e cole isto:

```
Adote a Diretriz GZero neste projeto existente.

Primeiro: copie TODO o conteúdo de
"C:\Users\artur\Área de Trabalho\Gzero\DiretrizDeProjetos\template"
para esta pasta — incluindo as pastas ocultas .projeto e .claude — SEM
sobrescrever nenhum arquivo que já exista aqui. Se já existir um CLAUDE.md,
mescle: as regras da Diretriz entram primeiro e o conteúdo antigo vira uma
seção "Notas específicas do projeto" no fim. Leia o CLAUDE.md resultante.

Depois faça a ADOÇÃO (ideação reversa):
1. Estude o projeto como ele está (código, README, git log se houver) e me
   diga em 5 linhas o que você entendeu que ele é.
2. Preencha pelo que leu: VISAO.md (o que o projeto é), PADROES.md (a stack e
   as convenções REAIS do código), ESTADO.md (onde está agora, como rodar) e
   ROADMAP.md — o que já funciona vira metas ✅ de um "Marco 0 — herdado";
   o que está pela metade ou faltando vira metas ⬜.
3. Só me pergunte o que NÃO dá para inferir do código (público, escopo,
   aparência desejada, o que fica de fora) — com opções prontas, como na
   Fase 1. Se o projeto tem interface e eu quiser mudar o visual, gere as
   direções em HTML; se eu gostar do visual atual, ele vira a referência
   travada.
4. Registre em DECISOES.md: as escolhas já feitas no projeto como TRAVADAS
   (são história — não se reabrem sem eu pedir) e as que dependem de mim
   como PENDENTES.
5. Siga para a Fase 2 (travamento) e, dali em diante, a Diretriz vale
   integralmente — inclusive a Preparação do repositório (.gitignore e git)
   se ainda não existirem.
```

Nas sessões seguintes desse projeto, é só dizer **continuar**, como em
qualquer outro.

## 1c. Atualizar um projeto antigo para a Diretriz atual

A Diretriz evolui. Para saber se um projeto está desatualizado, olhe a linha
`Versão da diretriz:` no topo do CLAUDE.md dele (projetos antigos nem têm essa
linha). Para atualizar, abra o Claude Code na pasta do projeto e cole:

```
Atualize este projeto para a versão atual da Diretriz GZero.

A versão mestre está em:
"C:\Users\artur\Área de Trabalho\Gzero\DiretrizDeProjetos\template"

Faça nesta ordem:

1. SUBSTITUA por completo (são metodologia, não conteúdo do projeto):
   - CLAUDE.md → pela versão do template. Se o atual tiver uma seção
     "Notas específicas do projeto", preserve-a no fim do novo.
   - .claude/settings.json → pela versão do template.

2. MESCLE os arquivos de .projeto/ (NUNCA apague conteúdo já preenchido):
   compare cada um com a versão do template e acrescente o que falta —
   seções novas, legendas, regras de cabeçalho. Em especial:
   - ESTADO.md: aviso "só o AGORA" + seção "Checkpoints para Artur"
   - ROADMAP.md: regras de ordenação/fatias verticais + seção "Correções"
     + nota nova de "Descobertas"
   - PADROES.md: toda seção que faltar (Sequência de verificação, Segredos,
     Segurança mínima, Dependências, Ambientes, Diretrizes de UX/UI com
     tokens, limpeza anti-inchaço, regressão/seed)
   - VISAO.md: "Exemplos de conteúdo real", contexto de uso
     (celular/computador) e "Sucesso é..." em formato verificável — o que
     não der para inferir do projeto, me pergunte com opções prontas
   - DECISOES.md: bloco de regras novo · diario/: seção "Caminhos descartados"

3. CHEQUE as obrigações novas que valem retroativamente:
   - .gitignore com `.env*` + `!.env.example`; confirme com git ls-files que
     nenhum .env está rastreado
   - repositório PRIVADO no GitHub: se não existir, crie
     (gh repo create <nome> --private --source=. --push); se existir, confira
     que é privado e faça push
   - se o projeto tem interface e não há direção visual travada nem tokens:
     NÃO refaça o visual — registre o visual ATUAL como referência travada
     e derive os tokens dele para o PADROES.md
   - se não existe estrutura de testes: crie a meta "estrutura de testes +
     smokes das metas já entregues" no início do próximo marco

4. NÃO reabra metas ✅ nem decisões travadas: as regras novas valem daqui em
   diante. Registre a atualização em DECISOES.md (DECIDIDA POR CLAUDE:
   "projeto atualizado para a Diretriz versão AAAA-MM-DD"), atualize o
   ESTADO.md e escreva a entrada do diário.

5. Ao terminar, me diga em até 10 linhas o que mudou e o que ficou pendente —
   e continue o trabalho de onde o projeto parou.
```

## 2. Retomar um projeto (o mais comum)

Abra o Claude Code na pasta do projeto e diga apenas:

```
continuar
```

A sessão lê o estado, anuncia onde o projeto está e segue trabalhando sozinha.

## 3. Ver a situação sem mexer em nada

```
status
```

O Claude relata: fase atual, o que já foi feito, o que está em andamento e o que
falta — sem alterar nada.

## 4. Pedir algo novo no meio do desenvolvimento

Fale normalmente, como pediria a alguém do seu time:

```
quero um botão para exportar a lista em PDF
```

O pedido vira uma meta, passa pelo mesmo loop de qualidade e depois o Claude
volta ao roadmap. Se o pedido esbarrar em algo que foi travado (por exemplo,
mudar o visual escolhido ou algo que ficou fora do escopo), o Claude primeiro
te mostra em 3 linhas o que muda e pergunta se você confirma — aí é só dizer sim.

## 5. Mudar uma decisão travada

Decisões travadas nunca são reabertas pelo Claude — só por você, assim:

```
quero destravar a decisão [assunto]. Nova direção: [o que você quer agora]
```

O Claude registra a mudança em DECISOES.md, avalia o impacto no que já foi
construído, ajusta o ROADMAP e segue.

---

## O que VOCÊ faz em cada fase (resumo)

| Fase | Seu papel | Tempo seu |
|------|-----------|-----------|
| 1 — Ideação | Responder as perguntas do Claude (ele oferece opções prontas) e escolher entre 2–3 propostas visuais que ele gera em HTML | 20–50 min |
| 2 — Travamento | Bater o martelo na lista final de decisões | 5–15 min |
| 3 — Execução | Nada. Só abrir novas sessões e dizer "continuar" quando pedido | ~0 |
| 4 — Entrega | Testar, dar feedback, aprovar publicação | Quanto quiser |

## Os checkpoints de marco (opcional, mas vale a pena)

A cada marco concluído, o Claude salva screenshots das telas em
`.projeto/screenshots/marco-N/` e te avisa — **sem parar de trabalhar**.
Olhar é opcional; mas quanto antes você reagir a algo que não gostou, mais
barato é corrigir. Seu feedback vira meta e entra no fluxo normal. Se você não
disser nada, ele simplesmente segue em frente.

## Quando a sessão chega perto do limite

Você vai receber exatamente esta mensagem:

> 🔄 **Cheguei perto do limite de contexto desta sessão.** Todo o progresso está
> salvo em `.projeto/` e no git.
>
> Abra uma nova sessão do Claude Code **nesta mesma pasta** e diga apenas: **continuar**

Faça isso e o desenvolvimento segue como se nada tivesse acontecido.

E se a sessão cair de repente, sem essa mensagem (janela fechada, queda de energia)?
Sem problema: o estado é salvo a cada meta concluída. Abra uma nova sessão e diga
**continuar** do mesmo jeito — no pior caso, perde-se só a meta que estava no meio.

## Se aparecer uma caixa em inglês pedindo permissão

O template já inclui um arquivo de permissões (`.claude/settings.json`) que
autoriza as operações comuns — editar arquivos do projeto, git, npm, node etc. —
para que o Claude trabalhe sem interromper você.

Mesmo assim, alguma ferramenta nova pode disparar uma pergunta do tipo
**"Allow Claude to run ...?"**. Isso é o aplicativo Claude Code (não o projeto)
pedindo autorização. Para operações dentro da pasta do projeto, escolha
**"Yes/Allow, don't ask again"** e o desenvolvimento segue. Na dúvida sobre algo
que pareça fora do projeto, pergunte ao próprio Claude o que aquilo significa.
