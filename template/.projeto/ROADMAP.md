# ROADMAP — metas do projeto

> Legenda: ⬜ não iniciada · 🟨 em andamento · 🟥 bloqueada (causa em ESTADO.md) · ✅ concluída (verificada e revisada)
>
> Uma meta só vira ✅ quando cumpre TODOS os critérios de aceite e passou pelo
> loop de qualidade completo (verificar rodando, incluindo caminho triste →
> revisar código → revisar UX → re-verificar se as revisões mudaram código).
> Meta trivial pode dispensar as revisões (ver "Cerimônia proporcional" no
> CLAUDE.md) — a verificação rodando, nunca.
>
> **Regra de ordenação:** o Marco 1 é sempre a menor versão do produto que Artur
> consegue abrir e usar de ponta a ponta (esqueleto navegável, mesmo raso, com
> dados de exemplo) — infraestrutura entra só na medida necessária para isso.
> Todo marco termina em algo demonstrável, nunca em trabalho puramente interno.
> Cada meta de funcionalidade é uma **fatia vertical**: entrega um caminho
> completo (tela → lógica → dados), nunca uma camada isolada que "vai servir
> depois". Metas de correção (FIX/FIX-DEP) e de refatoração são a exceção
> prevista.
>
> **Ordem de trabalho:** 1º meta 🟨 em andamento · 2º pedidos diretos de Artur ·
> 3º metas da seção Correções (FIX) · 4º a próxima meta na ordem em que aparece.

## Marco 1 — [nome do marco, ex.: MVP funcional]

### ⬜ M1.1 — [nome da meta]

**O que é:** [descrição em 1–2 frases]

**Critérios de aceite:**
- [ ] [critério verificável 1 — algo que dá para testar rodando o projeto]
- [ ] [critério verificável 2]

### ⬜ M1.2 — [nome da meta]

**O que é:** ...

**Critérios de aceite:**
- [ ] ...

## Marco 2 — [nome]

...

## Correções (bugs em metas já ✅ e vulnerabilidades)

> Prioridade acima de qualquer meta nova — bug em funcionalidade entregue vem
> antes de funcionalidade nova. Bug em meta ✅ vai direto para cá (nunca para
> Descobertas). Formato: `FIX-Mx.y-a — <resumo>`, com primeiro passo
> obrigatório: um teste automatizado que reproduz o bug e falha.
> Vulnerabilidade crítica/alta de dependência entra como `FIX-DEP-a` — sem o
> passo do teste; o critério é a auditoria limpa após atualizar, com a suíte verde.

- (nenhuma ainda)

## Descobertas (surgiram durante a execução)

> Só dívida técnica e ideias — bug em meta ✅ NÃO entra aqui (vai direto para
> Correções). Dois tipos, triados na Revisão de Marco: **dívida técnica** (algo
> que põe metas do roadmap em risco → Claude executa) e **SUGESTÃO PARA ARTUR**
> (funcionalidade nova que amplia o produto → só com pedido dele). Teste de uma
> linha: "se eu não fizer isso, alguma meta quebra ou fica em risco?" — se não,
> é sugestão.

- (nenhuma ainda)
