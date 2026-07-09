# GUIA DE PROMPTS — Estilo Gravidade Zero (Gzero)

> Manual da **célula rápida** para gerar artes por IA **indistinguíveis** das feitas pelo time de design.
> Estrutura e explicações em **pt-BR**; **todos os prompts em INGLÊS** (os modelos entendem melhor).
> Base: destilação forense dos 2 livros (250 págs) + PPTX "Humanware" (629 mídias) + tokens vetoriais determinísticos.

**Regra de ouro da casa:** o estilo Gzero **não é um filtro, é uma gramática impressa**. Ele nasce de serigrafia/risografia de poucas tintas, meio-tom (halftone) no lugar de gradiente, e traço de pincel feito à mão. A IA gera o **desenho**; a textura de impressão e **toda a tipografia** entram no pós (ver §7). Nunca confie na IA para render de texto — use as fontes reais.

---

## 0. Os dois modos (decida antes de escrever o prompt)

Todo o universo Gzero vive em **duas peles reversíveis**. Escolha uma; nunca misture as duas paletas na mesma peça.

| | **EDITORIAL CLARO** | **NEON ESCURO** |
|---|---|---|
| Fundo | creme `#FFF7EF` (texto) / branco `#FFFFFF` (ilustração riso) | preto `#080808`–`#231F20` / ameixa `#210D1F` |
| Tintas | magenta + amarelo-processo + vermelho-overprint sobre branco; nanquim preto | magenta + verde-lima + verde-menta neon + roxo + amarelo-ácido + vermelho-pop, com glow |
| Traço | nanquim preto modulado à mão (cartum) OU contorno magenta | contorno **colorido** (magenta/lima), nunca preto; ou branco knockout |
| Textura | halftone de pontos, escamas seigaiha, hachura, spray, grão de papel | halftone + grão VHS + glow/bloom + aberração cromática + colagem dadá |
| Sensação | livro de fábula, caloroso, arejado, tri-tonal | pôster punk-rave, alta-voltagem, colagem-sticker |
| Onde domina | miolo dos livros (~60-65%) | aberturas/clímax dos livros (~20%) + quase todo o PPTX |

**Constantes das DUAS peles** (a espinha dorsal que nunca muda):
- Rosa choque `#EC008C` como cor-assinatura onipresente.
- **Sombreamento só por meio-tom / halftone / stipple — jamais gradiente digital suave.**
- Traço de pincel/marcador modulado, trêmulo, pontas afiladas que ultrapassam os vértices.
- Universo **corte real + circo**: Bobo da Corte/elfo, gorro de guizos, gola de babados, coroa, estrela de 8 pontas, coração rabiscado.
- Acabamento de impressão suja: registro frouxo (off-register), respingos, contorno branco de adesivo, grão.

---

## 1. STYLE CORE — bloco mestre de estilo

Cole **um** destes três blocos em qualquer prompt. Eles carregam o DNA; você só acrescenta o assunto.

### 1.1 Bloco mestre (~110 palavras) — use quando quiser fidelidade máxima

```
Gravidade Zero house style: a hand-printed risograph / silkscreen zine aesthetic in
2 to 4 spot colors, anchored by shocking hot-magenta #EC008C. Every value is built from
halftone dot shading and stipple — never smooth digital gradients. Bold hand-inked brush
outlines with wobbly, pressure-modulated, tapering strokes that overshoot the corners;
thick white sticker cut-out edges; deliberate off-register overprint where magenta crosses
process-yellow into orange-red. A whimsical royal-court-jester and vintage-circus universe
with cosmic-pop motifs: eight-point stars, crowns, hearts, hand-drawn sparkles. Ink specks,
spray grain, visible paper texture, misregistration. Tender yet mischievous, DIY punk
editorial, high contrast, few colors, rich texture, controlled maximalist collage.
```

### 1.2 Versão curta (~25 palavras) — para prompts já longos

```
Gzero style: risograph zine in hot-magenta #EC008C, halftone dots not gradients,
wobbly hand-inked brush outlines, white sticker cut-outs, off-register overprint,
jester-circus cosmic-pop motifs, tender punk editorial.
```

### 1.3 Versão token (~8 palavras) — para encadear ou como sufixo de MJ

```
hot-magenta risograph jester-circus zine, halftone, hand-inked, off-register
```

> **Dica de peso:** em Midjourney, coloque a versão token no fim e controle a força com `--stylize`. Em Flux/SDXL, a versão curta funciona melhor como cauda do prompt principal. Em gpt-image-1 e Imagen, use o **bloco mestre completo** — eles seguem instrução longa e precisam do reforço explícito de "no gradients / printed halftone".

---

## 2. Variantes por modo (blocos próprios)

### 2.1 EDITORIAL CLARO (nanquim + creme + rosa)

Anexe ao bloco mestre (ou use sozinho para peças de livro):

```
--- MODE: Gzero EDITORIAL LIGHT ---
Warm cream paper background #FFF7EF (or pure white #FFFFFF for the illustration stage).
Two graphic dialects, never mixed within one mark:
(1) black nanquim/brush cartoon outline, modulated thick-to-thin, faces / gloved hands /
    curled-toe boots in clean 1930s-50s rubber-hose cartoon line;
(2) loose magenta fineliner/marker sketch for margin doodles.
Fills are flat magenta #EC008C rendered as halftone dots (round-dot and checkerboard),
with process-yellow #FFE500 line-art figures and orange-red #F0301E where inks overprint.
Occasional teal #00AAB3 for hand-written margin notes and translucent purple #9643FC as a
reader's highlighter. Airy negative space, single narrow text column, storybook-fable calm.
Risograph / silkscreen finish, seigaiha fish-scale waves for water, no smooth gradients.
```

**Assinaturas do modo claro** (peça uma ou mais explicitamente): contorno branco grosso de adesivo; halo de giz amarelo-limão em rabisco; escamas *seigaiha* para água; halftone xadrez (coração kawaii); marginália teal girada 90° ligada por seta curva à mão; poema-fantasma translúcido rotacionado sobre a arte.

### 2.2 NEON ESCURO (collage neon sobre preto)

```
--- MODE: Gzero DARK NEON ---
Pure black stage background #080808 (or aubergine-plum #210D1F), everything glowing on black.
Sticker-collage / punk cut-out composition, elements floating with soft neon glow and bloom.
Palette: hot-magenta #EC008C + acid lime-green #A8C838 + neon spring-mint #68F8A8 +
deep purple #483868 + acid yellow #F8F8A8 + neon-red pop #E84838. Colored (never black)
modulated brush outlines; white knockout for line-art on black. Duotone-recolored 19th-century
engravings (tone from dot density only), Dada photomontage cut-outs with rough scissor edges,
pink synthwave perspective grid, VHS color-noise specks, chromatic-aberration fringing, heavy
risograph film grain. Canonical type-emphasis pair: acid-yellow #F8F8A8 + magenta on black.
High-voltage, maximalist, editorial-punk keyvisual. Tone built by halftone, no smooth gradients.
```

**Assinaturas do modo neon** (peça explicitamente conforme o caso): recolor neon de gravura antiga (magenta puro sobre preto); duotone de foto (menta `#86CE8E` nas luzes + magenta/vinho nas sombras — a "gzerização"); molduras ovais vitorianas recoloridas com recorte lo-fi sujo; grade synthwave em perspectiva; blobs glossy rosa com halftone; rabiscos conectores em amarelo-limão neon `#F7FF50`.

> **Ressalva honesta:** verdes-lima, menta-neon e vermelho-pop **não constam da paleta vetorial oficial** — são acentos exclusivos do modo escuro (o núcleo confirmado é `#EC008C / #9643FC / #00AAB3 / #FFF7EF / #231F20`). Use-os no neon com liberdade, mas não os leve para peças institucionais claras.

---

## 3. Paleta como prompt (hex + descrição, por modelo)

### 3.1 Tokens de marca (verdade de base — valem nos dois modos)

| Papel | Hex | Nome em inglês para prompt |
|---|---|---|
| Rosa choque primário | `#EC008C` | `shocking hot-magenta / hot pink` |
| Creme editorial | `#FFF7EF` | `warm editorial cream / off-white paper` |
| Preto de impressão | `#231F20` | `warm print-black (never pure #000000 in light mode)` |
| Branco | `#FFFFFF` | `paper white / knockout white` |
| Roxo | `#9643FC` | `brand purple / translucent lilac highlighter` |
| Teal | `#00AAB3` | `editorial teal` |
| Rosa médio (raro) | `#EF5BA1` | `mid-pink blush` |
| Rosa pastel (raro) | `#FCDFEB` | `pale pastel pink` |

### 3.2 Acentos fora da paleta vetorial (estimados — tintas de ilustração)

Duas famílias distintas por modo — **não** as troque de lado:
- **Riso claro (2ª/3ª tinta das ilustrações do miolo):** `process/canary yellow ~#FFE500` · `overprint red-orange ~#F0301E` (surge onde magenta cruza amarelo). São as tintas das figuras-fábula amarelas e da sobreimpressão nas páginas claras (ex. `livro12-pag091`), **não** do neon escuro.
- **Neon escuro:** `acid lime-green #A8C838` · `neon spring-mint #68F8A8` · `deep purple/indigo #483868` · `acid pale-yellow #F8F8A8` · `neon-red pop #E84838` · `lime-yellow doodle-connector #F7FF50`.

### 3.3 Como escrever a cor em cada modelo

- **Midjourney v7:** não trava em hex; ele lê **nomes + referência**. Use nomes de cor fortes ("shocking hot-magenta, acid lime") e **ancore com `--sref`** de uma obra-chave. Reforce com `--no pastel, muted colors` se ele desbotar.
- **Flux / SDXL:** aceita hex razoavelmente **se houver caption/LoRA treinada**. Escreva `hot-magenta (#EC008C)` no prompt e repita o token de cor 1-2×. Sem LoRA, prefira nomes + um IP-Adapter de cor.
- **gpt-image-1:** é o **melhor em obedecer hex explícito**. Liste as cores como paleta fechada: `Use ONLY this palette: hot-magenta #EC008C, cream #FFF7EF, print-black #231F20, and process-yellow #FFE500 for overprint. No other hues.`
- **Imagen 4 / Gemini:** entende hex, mas **satura demais** — peça `slightly desaturated risograph inks, not glossy` e nomeie as cores. Ótimo para reforçar via edição/inpainting depois.

---

## 4. Negative prompts / o que suprimir

O estilo Gzero morre quando fica "limpo demais". Suprima agressivamente o vocabulário de **stock corporativo** e de **AI slop**.

**Lista canônica (o que NÃO queremos):**

```
smooth 3D gradients, corporate gradient mesh, glossy vector gradient, soft airbrushed bevel,
emboss, drop shadow, generic flat design, Corporate Memphis / Alegria big-limbed flat people,
Memphis-style 80s squiggles as the whole look, clip-art, stock illustration, cutesy vector mascot,
plastic 3D render, octane render, hyperrealistic, photographic skin (for illustrations),
clean uniform vector edges, perfectly symmetric, over-rendered, airbrush, lens flare,
rainbow gradient, pastel muted palette, watermark, signature, UI frame, alpha checkerboard,
AI slop, waxy shading, cinematic volumetric lighting.
```

**Como aplicar por modelo:**
- **Midjourney:** `--no smooth gradient, 3d render, corporate flat design, clip art, watermark, glossy` (o `--no` aceita lista curta; priorize os 5-6 piores para a peça).
- **SDXL / Flux:** cole a lista inteira no campo **negative prompt**.
- **gpt-image-1 e Imagen/Gemini:** **não têm** campo de negative prompt. Converta em **exclusões positivas** dentro do prompt: *"Flat printed risograph, absolutely no smooth gradients, no 3D, no glossy corporate look, no drop shadows; tone must come only from visible halftone dots on textured paper."*

---

## 5. Notas por modelo (forças e fraquezas para ESTE estilo)

### 5.1 Midjourney v7 — melhor para textura, pior para controle
**Forças:** halftone, riso, grão, pincel modulado e colagem saem lindos "de fábrica"; excelente atmosfera punk-editorial.
**Fraquezas:** hex exato e tipografia legível (nunca deixe o MJ escrever texto).

Parâmetros úteis:
- `--sref <URL>` — **a alavanca mais poderosa.** Aponte para obras-chave reais como referência de estilo. Combine várias com pesos: `--sref urlA::2 urlB::1`. (Hospede os PNGs da pasta `00-Material-Extraido` num link acessível.)
- `--sref random` — para explorar variação mantendo a "família".
- `--sw 0-1000` (style weight) — quanto o sref manda; comece em `--sw 250-500`.
- `--cref <URL> --cw 0-100` (character reference) — **consistência do Bobo** entre poses; use `--cw 100` para roupa+rosto, `--cw 30` só para o rosto. (v7 também aceita omni-reference/`--oref`.)
- `--p <code>` (personalization) — se a célula treinar um perfil só com curadoria Gzero, ative com `--p` para enviesar todo o feed ao gosto da casa.
- `--stylize 50-1000` — baixo (`--s 50-150`) obedece mais ao prompt; alto embeleza (risco de "bonito genérico"). Para Gzero fique em `--s 100-300`.
- `--chaos 0-30` para variedade de composição; `--ar 1:1` (livro), `16:9` (slide), `9:16` (story/hero).

srefs recomendados (obras-mãe): capa `livro12-pag001.png`, mosaico neon `image8.png`, bobo pintado `image244.png`, colagem-herói `image450.png`, duotone riso `livro3-pag034.png`.

### 5.2 Flux / SDXL — melhor para REPETIÇÃO em escala → **treine um LoRA**
Para produção industrial e coerência, **treine um LoRA** (ou dois: um por modo) com as obras-chave como dataset. É o caminho mais confiável para "indistinguível".

**Dataset sugerido (LoRA de estilo):**
- 40-80 imagens curadas, **separadas por modo** (não misture claro e neon num mesmo LoRA se quiser controle — treine `gzero_light` e `gzero_dark`).
- Claro: `livro12-pag029/041/057/068/091/101`, `livro3-pag012/034/040/058`, `image257`, `image487-490`.
- Neon: `image8`, `image244`, `image450`, `image4`, `image334`, `image384`, `image359`, `image281`, `image299`, `image396.svg` (rasterizado).
- **Caption template** com token-gatilho consistente: `gzero_light style, <descrição objetiva>, hot-magenta halftone, hand-inked brush outline, cream paper, risograph` (e `gzero_dark style, ...` para o outro). Descreva o conteúdo, não o estilo (o LoRA aprende o estilo).
- Base: **Flux.1-dev** rende halftone/grão melhor que SDXL base; SDXL 1.0 + refinamento tende a alisar — compense com o negative prompt inteiro.

**Fluxos de controle:**
- **ControlNet (canny/lineart)** para impor layout de spread/moldura.
- **IP-Adapter** para transportar a paleta ou o rosto do Bobo.
- LoRA de estilo `--strength 0.7-0.9`; passe a lista de negatives inteira.

### 5.3 gpt-image-1 — melhor para OBEDIÊNCIA e colagem descrita
**Forças:** segue instrução longa e **paleta hex fechada**; monta colagens complexas descritas em palavras; bom para composições com muitos elementos nomeados (modo neon).
**Fraquezas:** tende ao **liso/renderizado ("AI slop")** — precisa de pressão explícita por halftone e grão; render de texto passável, mas **ainda assim componha a tipografia real** no pós.
**Receita:** bloco mestre completo + paleta fechada (§3.3) + exclusões positivas (§4) + "tone only from visible halftone dots, printed on textured paper, slightly off-register".

### 5.4 Imagen 4 / Gemini ("Nano Banana") — melhor para DUOTONE e edição
**Forças:** trata foto em duotone/risograph com naturalidade (ideal para a receita "foto gzerizada"); **edição conversacional/inpainting** forte para consertar detalhe; bom com pôster de circo.
**Fraquezas:** **satura e desvia a cor**; menos "sujeira" punk. Peça grão e registro frouxo explicitamente e valide o hex depois.
**Uso ideal na célula:** gerar a base de foto-duotone e fazer ajustes finos por edição, depois tratar no pós.

> **Resumo de escolha:** exploração e textura → **Midjourney** (com sref). Produção repetível e personagem consistente → **Flux/SDXL + LoRA**. Colagem descrita e paleta exata → **gpt-image-1**. Foto-duotone e edição → **Imagen/Gemini**.

---

## 6. O que a IA NÃO deve fazer (limites duros)

1. **Nunca gerar tipografia final.** Qualquer texto na imagem gerada é rascunho de layout — será mascarado e substituído por fonte real (§7).
2. **Nunca gerar logos de terceiros** (marcas de clientes). A convenção da casa é rebaixá-los a knockout branco/prata; isso é tratamento de asset existente, não geração.
3. **Nunca inventar o robô-mascote / "rádio JPL"** em cenas de livro — ele não aparece nos livros; só há o Bobo e coadjuvantes. No PPTX existe um mascote-robô estilo console de videogame (ANI), que é outra coisa.
4. **Evitar** o balão-de-chat roxo solto sobre a arte — nos fontes é, muitas vezes, resíduo de comentário de software, não design.
5. **Não usar gradiente digital suave** em lugar nenhum. Volume = densidade de pontos.

---

## 7. Workflow recomendado da célula rápida

Pipeline de 3 passos. A IA cobre **só o passo 1**. O que faz a arte virar "Gzero de verdade" está nos passos 2 e 3.

### Passo 1 — GERAR (IA)
- Escolha o modo (§0), monte o prompt: `STYLE CORE` + bloco de modo + assunto + paleta + negatives.
- Gere **sem depender de texto**; se precisar de espaço para título, peça "empty negative space top-left for a headline".
- Itere composição; exporte em alta (upscale). Guarde a versão limpa (sem grão) para tratar melhor.

### Passo 2 — TRATAR (pós-produção: halftone + grão + registro frouxo)
Adicione a **materialidade impressa** que a IA não entrega bem:
- **Halftone / meio-tom:** Photoshop → *Filter > Pixelate > Color Halftone* ou *Filter > Sketch > Halftone Pattern*; **Duotone** via *Image > Mode > Duotone* ou *Gradient Map*. Alternativas: **Affinity Photo** (Halftone live filter), **Procreate** (brushes de halftone), **Photopea** (grátis, tem Color Halftone), apps **Risotto / Halftone Pro / Mr. Halftone**.
- **Texturas riso reais:** packs da **True Grit Texture Supply** (Riso, Grit, Screen), overlays de **grão de papel** em *Multiply/Overlay*.
- **Off-register (registro frouxo):** separe canais por cor e desloque 2-6px cada tinta; deixe respingos e "chiado" nas bordas. É a assinatura mais reconhecível.
- **Contorno branco de adesivo:** *Layer Style > Stroke* branco grosso nas massas de cor (modo claro).
- **Neon escuro:** *Outer Glow* suave + grão VHS (specks R/G/B) + leve aberração cromática nas bordas.

### Passo 3 — COMPOR com TIPOGRAFIA REAL (nunca IA)
**Toda** a tipografia e o lettering usam as **fontes verdadeiras extraídas**, montadas em Figma / InDesign / Illustrator sobre a arte tratada:

Pasta dos subsets reais:
`C:\Users\artur\Área de Trabalho\Gzero\Design&ArtStyleGzero\GZERO-DESIGN-SYSTEM\03-Design-System\Fontes-Extraidas-dos-PDFs`

| Papel | Fonte (arquivo) | Uso |
|---|---|---|
| Título-marca carved | **AW Conqueror Std Carved** (`AWConquerorStdCarved-Regular.cff`) | "GRAVIDADE ZERO", títulos de fábula, efeito neon-marquise |
| Voz humana / lettering | **Salted** (`Salted-Regular.ttf`) | falas do Bobo, títulos de capítulo, marginália, pull-quotes |
| Display condensado/rótulo | **Tanker** (`Tanker-Regular.cff`) e **ADAM.CG Pro** (`ADAM.CGPRO.cff`) | rubricas, sumário, manifestos, rótulos de infográfico |
| Corpo de leitura | **Atkinson Hyperlegible** (`-Regular` / `-Bold` / `-Italic`) | todo texto corrido; itálico = rubrica cênica |
| Subhead slab | **Hepta Slab ExtraLight** (`HeptaSlab-ExtraLight.ttf`) | subtítulos slab pontuais |
| Tech / VHS | **Home Video** (`HomeVideo-Regular.ttf`) | disclaimers, tom glitch retrô |
| Código | **Menlo** / **Courier** (`Menlo-*`, `Courier.ttf`) | aparte ".código-aberto-com-alma" |

Regras de composição tipográfica (da própria diagramação dos livros):
- Título de capítulo = **Salted magenta** gigante, caixa-alta, baseline saltitante, 2-4 linhas.
- Marginália = **Salted teal** girada 90°, ligada ao corpo por **seta curva desenhada à mão**.
- Frase de maior peso é "promovida" do preto neutro para o **lettering rosa à mão**.
- Bloco de assinatura = nome em magenta (Atkinson) + cargo em display condensado preto.
- Sem líder de pontos no sumário: número preto colado ao fim do título branco.
- Mascare qualquer texto que a IA tenha gerado e substitua por essas fontes.

**Checklist de entrega (a peça está "indistinguível"?):**
- [ ] Sombreamento é 100% halftone/stipple — zero gradiente suave?
- [ ] Rosa é exatamente `#EC008C`?
- [ ] Traço tem tremor/pressão de pincel, pontas afiladas?
- [ ] Tem registro frouxo, respingos e grão de papel?
- [ ] Toda a tipografia é fonte real (não IA)?
- [ ] Motivo do universo corte/circo presente (bobo, guizo, estrela de 8 pontas, coração)?
- [ ] Nada de 3D liso, corporate flat, clip-art ou AI slop?

---

## 8. Referências rápidas de obras-mãe (para `--sref`, dataset de LoRA e conferência visual)

Raiz: `C:\Users\artur\Área de Trabalho\Gzero\Design&ArtStyleGzero\GZERO-DESIGN-SYSTEM\00-Material-Extraido\`

**Editorial claro:** `Livro-Gzero-1e2-Paginas\livro12-pag001.png` (capa/DNA) · `...\livro12-pag029.png` (Bobo canônico) · `...\livro12-pag057.png` (duplo-registro trapézio) · `...\livro12-pag101.png` (Bobo corpo inteiro) · `Livro-Gzero-3-Paginas\livro3-pag034.png` (duotone riso portas) · `...\livro3-pag012.png` (Bobo em salto).

**Neon escuro:** `Apresentacao-Humanware-Midia\image8.png` (mosaico-mãe) · `...\image450.png` (colagem-herói vertical) · `...\image244.png` (bobo pintado premium) · `...\image4.png` (elfos-lata + portal) · `...\image334.png` (fotomontagem dadá) · `...\image281.png` (DNA hero) · `...\image396.svg` (sapo mascote neon).

---

*Consulte `receitas-e-exemplos.md` (mesma pasta) para prompts completos, prontos para copiar, por tipo de artefato.*
