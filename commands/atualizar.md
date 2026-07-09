---
description: Atualiza um projeto que já usa a Diretriz GZero para a versão mais recente do template
---

Você vai atualizar este projeto para a versão atual da **Diretriz GZero**.

A versão mestre é a do plugin: localize a raiz (via `CLAUDE_PLUGIN_ROOT` ou
`~/.claude/plugins/marketplaces/diretriz-gzero/`) e use
`<raiz-do-plugin>/template/` como fonte. Compare a linha `Versão da diretriz:`
do CLAUDE.md do projeto com a do template — se forem iguais, diga que o projeto
já está atualizado e pare.

Faça nesta ordem:

1. **SUBSTITUA por completo** (são metodologia, não conteúdo do projeto):
   - `CLAUDE.md` → pela versão do template. Se o atual tiver uma seção
     "Notas específicas do projeto", preserve-a no fim do novo.
   - `.claude/settings.json` → pela versão do template.

2. **MESCLE os arquivos de `.projeto/`** (NUNCA apague conteúdo já preenchido):
   compare cada um com a versão do template e acrescente o que falta — seções
   novas, legendas, regras de cabeçalho. O que não der para inferir do projeto,
   pergunte ao dono com opções prontas.

3. **CHEQUE as obrigações que valem retroativamente:**
   - `.gitignore` com `.env*` + `!.env.example`; confirme com `git ls-files`
     que nenhum `.env` está rastreado.
   - Repositório PRIVADO no GitHub: se não existir, crie
     (`gh repo create <nome> --private --source=. --push`); se existir,
     confira que é privado e faça push.
   - Se o projeto tem interface e não há direção visual travada nem tokens:
     NÃO refaça o visual — registre o visual ATUAL como referência travada e
     derive os tokens dele para o PADROES.md.
   - Se não existe estrutura de testes: crie a meta "estrutura de testes +
     smokes das metas já entregues" no início do próximo marco.

4. **NÃO reabra metas ✅ nem decisões travadas**: as regras novas valem daqui
   em diante. Registre a atualização em DECISOES.md (DECIDIDA POR CLAUDE:
   "projeto atualizado para a Diretriz versão AAAA-MM-DD"), atualize o
   ESTADO.md e escreva a entrada do diário.

5. Ao terminar, resuma em até 10 linhas o que mudou e o que ficou pendente —
   e continue o trabalho de onde o projeto parou.
