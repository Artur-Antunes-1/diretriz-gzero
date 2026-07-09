# Design System GZero — pacote de sugestão visual

> Este pacote acompanha a Diretriz GZero como **sugestão, nunca obrigação**:
> na Fase 1 (Ideação), uma das direções visuais oferecidas pode nascer com a
> cara oficial da Gravidade Zero, pronta. O dono do projeto sempre escolhe.

Conteúdo (destilado do repositório GZERO-DESIGN-SYSTEM, fonte da verdade):

| Arquivo | O que é |
|---|---|
| `tokens.css` | Variáveis CSS `--gz-*` prontas para web — Modo A (Editorial Claro) e Modo B (Neon Escuro) |
| `tokens.json` | Os mesmos tokens em formato W3C Design Tokens |
| `design-system-gzero.md` | O design system completo: cores com nomes próprios, tipografia, combinações permitidas e proibidas, componentes |
| `estilo-artistico-gzero.md` | A direção de arte: o traço, os motivos, as texturas, os dois modos |
| `guia-prompts-gzero.md` | Receitas para gerar imagens no estilo GZero com IA |
| `fontes/` | Subsets das fontes livres da marca (Atkinson Hyperlegible — OFL, Hepta Slab — OFL, Home Video — freeware). **Salted** não pode ser redistribuída (licença Fontshare): baixe grátis em https://www.fontshare.com/fonts/salted ou use o CDN oficial (`https://api.fontshare.com/v2/css?f[]=salted@400`) |

## Regras de ouro do visual GZero (resumo para a IA que for usar)

1. **Rosa Spray `#EC008C` é a cor-mãe**, não um acento.
2. **Meio-tom no lugar de gradiente — sempre.** Nenhum degradê digital suave.
3. Dois modos que **se alternam, nunca se misturam** na mesma superfície:
   Editorial Claro (creme `#FFF7EF` + preto quente `#231F20`) para leitura;
   Neon Escuro (preto `#080808` + acentos ácidos) para impacto.
4. Corpo de texto sempre em **Atkinson Hyperlegible**; títulos afetivos em
   **Salted** (lettering à mão); display pesado em **Tanker**.
5. Acentos neon (lima, menta, brasa) **só sobre preto** — no claro ficam sujos.
6. Nunca `#000000` puro no editorial (use o Preto Prensa `#231F20`).
7. A voz manuscrita na margem (teal `#00AAB3`) e o grifo roxo translúcido são
   a assinatura de diagramação da casa.

Para o sistema completo e o site navegável, procure o repositório
GZERO-DESIGN-SYSTEM da empresa.
