# Diretriz GZero de Projetos

Sistema de desenvolvimento de projetos com Claude Code em que:

- **Artur decide O QUÊ** — a ideia, a aparência, as prioridades, o que entra e o que fica de fora.
- **Claude decide COMO e executa** — código, arquitetura, testes, revisão, UX, tudo.
- **Qualquer sessão nova se localiza sozinha** — basta abrir o Claude Code na pasta
  do projeto e dizer **continuar**.

## Como funciona (as 4 fases)

| Fase | Nome | Quem participa | O que acontece |
|------|------|----------------|----------------|
| 1 | Ideação | Artur + Claude | Conversa guiada para definir o projeto por completo — incluindo a escolha entre 2–3 propostas visuais em HTML que você abre no navegador |
| 2 | Travamento | Artur + Claude | Todas as decisões que dependem de Artur (incluindo a direção visual e o escopo) são fechadas e travadas |
| 3 | Execução autônoma | Só Claude | Claude desenvolve tudo em loops: meta → construir → verificar → revisar código → revisar UX → concluir. A cada marco concluído, deixa screenshots para você espiar (sem esperar resposta) |
| 4 | Entrega | Artur + Claude | Checklist de sucesso testado ✅/❌, demonstração, publicação e manutenção |

## Como começar um projeto novo

1. Crie uma pasta nova para o projeto (ex.: `Gzero/MeuApp`).
2. Abra o Claude Code nessa pasta.
3. Cole o prompt de **"Projeto novo"** que está em [COMO-INICIAR.md](COMO-INICIAR.md).

O próprio Claude copia o template para a pasta e inicia a ideação.

## Como retomar um projeto

1. Abra o Claude Code na pasta do projeto.
2. Diga: **continuar**

Só isso. A sessão lê os arquivos de estado e segue exatamente de onde a anterior parou.

## A memória do projeto (pasta `.projeto/`)

Todo projeto criado com este sistema tem uma pasta `.projeto/` que funciona como a
memória permanente — é ela que permite que sessões diferentes abram o mesmo projeto
e se localizem imediatamente:

| Arquivo | O que guarda |
|---------|--------------|
| `ESTADO.md` | Onde o projeto está AGORA — o relatório de passagem de bastão entre sessões |
| `VISAO.md` | O projeto inteiro: o que é, para quem, o que faz, como deve parecer |
| `DECISOES.md` | Tudo que foi decidido e travado (nunca reaberto sem sua autorização) |
| `ROADMAP.md` | As metas, em ordem, cada uma com critério claro de "pronto" |
| `PADROES.md` | Stack, convenções, qualidade, segurança, dependências e design tokens |
| `diario/` | Um relatório por sessão de trabalho (histórico completo) |
| `direcoes/` | As 2–3 propostas visuais em HTML geradas na ideação |
| `screenshots/` | As imagens de cada marco concluído — seus checkpoints |

Além dela, o template traz `.claude/settings.json`, que pré-autoriza as
operações comuns (editar arquivos, git, npm...) para que a execução autônoma
não pare em caixas de permissão.

## Regras de ouro do sistema

1. **Toda sessão começa lendo `.projeto/ESTADO.md`.** Sem exceção.
2. **Decisão travada não se reabre.** Só você pode destravar, pedindo explicitamente.
3. **Na Fase 3, o Claude não pede permissão** — ele executa e presta contas no
   ESTADO e no diário. Ele só interrompe você para: gastar dinheiro, apagar
   dados, publicar em produção, criar contas/credenciais externas, enviar código
   para qualquer lugar que não seja o repositório privado do projeto no GitHub
   (deploy mesmo de teste, outro serviço, tornar o repo público), decisões
   grandes que não dá para desfazer, ou algo que contrarie uma decisão travada.
4. **Nenhuma meta é concluída sem qualidade real**: verificação rodando de verdade +
   revisão de código + revisão de UX. (Exceção: meta trivial — corrigir um texto,
   por exemplo — pode dispensar as revisões; a verificação, nunca.)
5. **O ESTADO.md é atualizado a cada meta concluída** — nunca "depois". Assim, mesmo
   que a sessão caia de repente, quase nada se perde.
6. **Todo projeto vive num repositório privado no GitHub**, criado automaticamente
   na primeira sessão e atualizado com push a cada meta — backup fora do
   computador, sem você fazer nada. Se o projeto já tem repositório, ele só
   continua atualizando.
7. **Perto do limite de contexto (~90%)**, a sessão salva tudo com segurança e
   encerra com a mensagem padrão: *"abra uma nova sessão nesta pasta e diga: continuar"*.
