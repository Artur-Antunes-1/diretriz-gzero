# DESIGN SYSTEM GRAVIDADE ZERO

> Sistema visual oficial da Gzero — aplicável a **web, slides, editorial e social**.
> Versão 1.0 · pt-BR · Design Systems Lead
> Universo criado por **Dante Freitas** e **Renan Hannouche** — "Renante", a fusão dos dois nomes, é também o nome da IA da casa.
> Obra-fonte: *"O Mundo em Gravidade Zero — com amor & spray rosa"* (livros 1, 2 e 3) + deck *"Humanware por GZero"*.

Este documento é a **fonte da verdade** para quem projeta qualquer peça Gzero. Ele nasce de uma destilação forense de 250 páginas de livro, 629 mídias de apresentação e das cores e fontes extraídas por código dos arquivos originais. Os hex do **núcleo de marca** e as **fontes reais embutidas** são fatos determinísticos — prevalecem sobre qualquer estimativa.

Arquivos irmãos:
- `tokens.json` — design tokens (formato W3C Design Tokens).
- `tokens.css` — variáveis CSS `--gz-*` prontas para web, com modo claro e `[data-theme="dark"]`.
- `Fontes-Extraidas-dos-PDFs/` — subsets reais das fontes embutidas.

---

## 1. FUNDAMENTOS DA MARCA

### 1.1 Essência visual (em um parágrafo)

Gravidade Zero é um **fanzine punk vestido de édito real**: uma editora-manifesto que imprime ideias sérias sobre trabalho, tecnologia e afeto com a energia de um cartaz de circo dos anos 60 passado no risógrafo. Tudo gira em torno de uma cor — o **rosa choque** — e de um narrador, o **Bobo da Corte**, cuja voz manuscrita comenta, provoca e subverte o texto "oficial" na margem da página. O acabamento é sempre **feito à mão e impresso à mão**: contornos de pincel que tremem, meio-tom em vez de gradiente, registro de cor propositalmente frouxo, spray, grão e recorte de adesivo. É maximalista mas caloroso, irônico mas terno — "com amor & spray rosa". A assinatura mais profunda da marca não é um logo: é a **convivência de duas peles**, a voz institucional e a voz do bufão, o preto-e-creme da leitura e o neon sobre o breu.

### 1.2 Os DOIS MODOS

A marca opera em dois modos reversíveis. **Não são temas claro/escuro de UI** — são duas atmosferas editoriais com propósitos diferentes. Uma peça pertence a um modo; a força do sistema está em **alternar** entre eles (o "inspira/expira" do livro), nunca em misturá-los na mesma superfície.

#### MODO A — EDITORIAL CLARO ("a página")
Creme + preto quente + rosa choque. É o modo da **leitura, do argumento, da confiança**. Fundo creme `#FFF7EF`, corpo em Atkinson Hyperlegible preto, títulos em lettering rosa à mão, marginália teal. Calmo, arejado, altíssima legibilidade, muito espaço em branco. Riso e halftone entram só nas ilustrações.

> **Use quando:** texto longo, corpo editorial, posts de reflexão, páginas "sobre", documentação, e-mails, PDFs de leitura, qualquer peça em que a palavra pesa mais que a imagem. É o **default** para conteúdo textual.

#### MODO B — NEON ESCURO ("o palco")
Preto de palco + rosa neon + acentos ácidos (lima, menta, roxo, âmbar). É o modo do **impacto, do clímax, da colagem**. Fundo preto `#080808`, arte-sticker recortada, halftone denso, glow neon, grade synthwave, personagens em duotone. Alta saturação, alto contraste, horror-vacui controlado. "Apaga a luz e acende o neon."

> **Use quando:** capas, aberturas, títulos de impacto, slides-herói, stories, cards de destaque, lançamentos, o momento em que o Bobo "entra em cena". É o modo de **atenção**, não de leitura longa.

**Regra de ouro:** dentro de uma mesma peça ou sequência, os modos se **alternam** para criar ritmo (uma abertura neon → miolo claro → um respiro preto → clímax neon). O contraste entre eles é a batida visual central da marca. Uma terceira superfície — **neon sobre branco** (riso-collage) — é um sub-modo das ilustrações: a arte neon posta sobre `#FFFFFF` puro em vez de preto.

### 1.3 Um sub-sistema à parte: "Humanware / Direito" (oliva)
O material contém um **sistema de produto (SaaS jurídico)** em creme + **verde-oliva** `#5B6A1C`, sóbrio e acessível. Ele **não usa o rosa da marca** e não é comunicação institucional. Está documentado aqui apenas para que ninguém o force ao magenta: quando desenhar telas desse produto, use a sub-paleta oliva (seção 2.5), não o modo neon.

---

## 2. CORES

### 2.1 Núcleo de marca (verdade de base — hex vetoriais confirmados)

Oito cores. São as únicas que valem em **impressão** e em **tela** sem ressalva. Todo o resto é acento ou estimativa.

| Nome próprio | Hex | Papel semântico | Onde vive |
|---|---|---|---|
| **Rosa Spray** | `#EC008C` | Cor-assinatura, onipresente | Títulos, lettering do Bobo, contornos, molduras, campos chapados, ênfase. A "tinta" da casa. |
| **Creme Editorial** | `#FFF7EF` | Fundo de leitura (Modo A) | Papel de toda página de texto; reserva/luz nas ilustrações. |
| **Preto Prensa** | `#231F20` | Texto + traço + fundos escuros mornos | Corpo Atkinson; nanquim; fundo escuro "quente". **Nunca `#000000` puro** no editorial. |
| **Branco Reserva** | `#FFFFFF` | Palco das ilustrações / knockout | Fundo do sub-modo riso-collage; line-art sobre neon; logos knockout; rostos e luvas. |
| **Roxo Realce** | `#9643FC` | Grifo de leitor + stickers | Marca-texto translúcido sobre 1–3 palavras; etiquetas; ícones de balão. |
| **Teal Marginália** | `#00AAB3` | Voz manuscrita da margem + setas | Notas do Bobo/autor rotacionadas 90°; setas curvas à mão; voz "código-com-alma". |
| **Rosa Blush** | `#EF5BA1` | Acento raro / bochecha / meio-tom | Blush dos personagens; halftones rosados; itálico de narração. |
| **Rosa Névoa** | `#FCDFEB` | Fundo suave / halftone claríssimo | "Tela de sistema"; holofotes; retículas muito claras. |

**Tints canônicos do Roxo Realce** (mesma cor, opacidade variável, para marca-texto): `#C9A6F5`, `#D9C6F2`. A variação é de opacidade sobre creme, não de matiz.

### 2.2 Paleta do Modo Neon Escuro (o "palco")
Tratada como **conjunto próprio e canônico do Modo B** — extraída por clustering das artes do deck. O Rosa Spray continua sendo a espinha dorsal; estes entram como fundo e acentos ácidos que **só existem sobre preto**.

| Nome próprio | Hex | Papel |
|---|---|---|
| **Preto Palco** | `#080808` | Fundo dominante do Modo B (mais fechado que o Preto Prensa). |
| **Rosa Neon** | `#E838A8` | Família rosa-choque quente do neon (`#D83888`–`#E838A8`); glow, contornos emissivos. |
| **Lima Ácida** | `#A8C838` | Verde-limão de alta voltagem: lettering marcador, contornos punk, duotone. |
| **Menta Fantasma** | `#68F8A8` | Verde-menta neon: golas de bobo, DNA, olhos, auras halftone. |
| **Índigo Noite** | `#483868` | Roxo profundo: sombras, mantos, grades, badges. |
| **Brasa** | `#E84838` | Laranja-vermelho: pop pontual, chamas, acentos quentes. |
| **Poeira de Estrela** | `#F8F8A8` | Amarelo pálido: sparkles, glow suave, poeira cósmica. |

> **Nota de honestidade:** lima, menta, índigo, brasa e poeira **não constam da paleta vetorial oficial** — são acentos exclusivos do modo escuro, canonizados aqui para dar consistência ao Modo B. Use-os com parcimônia (acento, não base). Rosa e roxo do neon batem com os oficiais; os demais são clusters de tela.

### 2.3 Tintas de ilustração (riso/serigrafia — ESTIMADAS, fora da marca)
Aparecem **só dentro das pranchas ilustradas full-bleed**, nunca como cor de interface, texto ou fundo de peça. São aproximações de raster com meio-tom — **não crave um hex único**; pense "canary yellow", "overprint red".

| Faixa | Hex de referência | Papel |
|---|---|---|
| **Amarelo Processo** | `~#FFE500` | 2ª tinta riso: sol, cometa, raios, contornos de figura-fábula, halftone quente. |
| **Vermelho Overprint** | `~#F23A1E` | Onde magenta cruza amarelo (sobreimpressão): chamas, água, corações. |
| **Laranja Riso** | `~#F7941E` | Gradação intermediária do overprint. |
| **Ciano Respingo** | `~#00AEEF` | Capacete do astronauta, íris, respingos fora de registro. |
| **Azul-Fantasma** | `~#6E7FC4` | Camada de "poema-fantasma" translúcido sobre ilustrações (propositalmente ilegível). |

### 2.4 Proporções de uso (regra prática)
- **Modo Editorial Claro ≈ 60–65%** do volume · **Neon Escuro ≈ 20%** · **pranchas ilustradas full-bleed ≈ 15%**.
- No claro: o **preto** é a maior massa (corpo de texto), mas o **rosa é a cor de assinatura** — moldura, título, voz do Bobo. Teal e roxo entram como **acentos cirúrgicos** (1–2 ocorrências por página).
- No neon: **rosa domina** (>60% das peças o trazem como cor principal ou contorno); **preto** é o palco; **roxo** é o secundário universal; verdes são o terceiro grupo (acento/duotone); âmbar, brasa e vermelho são pontuais.

### 2.5 Sub-paleta "Humanware / Direito" (produto — oliva, NÃO é marca)
Só para telas do produto jurídico. Nunca migrar para comunicação institucional.
`Oliva Humanware #5B6A1C` (acento) · `Creme Produto #FBF9F1` (fundo) · `Grafite Rótulo #2E2A24` · `Cinza Morno #6F6F6F` (secundário) · `Borda Clara #E7E3D9`.

### 2.6 Combinações permitidas e proibidas

**Permitidas (assinatura):**
- Rosa Spray sobre Creme Editorial (título rosa em página clara).
- Preto Prensa sobre Creme Editorial (corpo de leitura).
- Teal Marginália e Roxo Realce sobre Creme, **em pequena dose**.
- Rosa Spray / Branco / acentos neon sobre Preto Palco (modo escuro).
- Branco Reserva (line-art) sobre campo chapado de Rosa Spray.
- Rosa Spray chapado como campo inteiro com arte preta (capa livro 1e2) — e o inverso, preto com arte rosa (capa livro 3). **A inversão é intencional e é marca.**

**Proibidas:**
- Rosa Spray sobre Roxo Realce, ou Teal sobre Rosa — **vibração ilegível**, sem contorno branco entre eles.
- Acentos neon (lima, menta, brasa) sobre fundo creme claro — só brilham sobre preto; no claro ficam sujos.
- `#000000` puro como fundo do Modo A (use Preto Prensa `#231F20`, quente).
- Oliva Humanware misturado ao rosa da marca na mesma peça.
- Gradiente digital suave como preenchimento (ver seção 6 — volume é sempre por textura).
- Tintas de ilustração (amarelo/vermelho riso) usadas como cor de UI, texto ou fundo.

### 2.7 Tela vs. impressão
- **Tela:** use os hex exatamente como listados (sRGB). No Modo B, `#080808` como fundo; permita glow/bloom (só existe em tela).
- **Impressão:** Rosa Spray é um **spot color** (equivalente a Pink 806 / magenta forte) — não confie no CMYK de processo para reproduzi-lo; especifique Pantone quando possível. Preto de texto é o **Preto Prensa quente** `#231F20`, não preto de registro. O "neon" impresso vira **serigrafia/risografia de 2–4 tintas** com registro frouxo — o glow de tela vira halftone e overprint. Amarelos e vermelhos de ilustração são tintas spot riso, não CMYK.

---

## 3. TIPOGRAFIA

Oito famílias reais, embutidas nos arquivos-fonte. Cada uma é uma **voz**, não só um estilo. A assinatura tipográfica da marca é o **duplo registro**: texto sério (Atkinson) contraposto à glosa manuscrita (Salted) que comenta e subverte.

### 3.1 As famílias e seus papéis

| Família | Papel | Onde obter |
|---|---|---|
| **Atkinson Hyperlegible** (Regular/Bold/Italic) | **Corpo de leitura.** A voz-narrador racional. Todo texto corrido, legendas, UI, fólios. | Google Fonts (grátis, OFL). |
| **Tanker** | **Display condensado pesado.** Rubricas de seção, sumário, títulos "gordos" de circo, letreiros. | Fontshare (grátis). |
| **Salted** | **Lettering à mão.** A voz humana / do Bobo. Títulos narrativos, pull-quotes, marginália, assinaturas. | Fontshare (grátis). |
| **AW Conqueror Std Carved** | **Display carved/inline.** Wordmark "GRAVIDADE ZERO", títulos de abertura de parte/fábula, efeito neon-marquise. | Licenciada (Typofonderie). |
| **Hepta Slab ExtraLight** | **Slab de detalhe.** Kickers, fólios display, microtipografia editorial fina; contraponto elegante ao peso do carved. | Google Fonts (grátis). |
| **Home Video** | **Mono VHS retrô.** Tom tech-glitch, disclaimers, "desconfigure suas configurações de fábrica". | Freeware. |
| **ADAM.CG Pro** | **Condensada display alternativa.** Rótulos industriais/pôster, subheads de impacto quando o carved não cabe. | Licenciada (freeware p/ uso pessoal; checar licença comercial). |
| **Menlo / Courier** | **Monoespaçada / voz de máquina.** O aparte `.código-aberto-com-alma-GZero{ }`, blocos de código, CIP. | Sistema (Menlo/macOS; Courier ubíquo). Alternativa livre: JetBrains Mono. |

> **Fallback web seguro:** se uma licenciada não estiver disponível, degrade assim — Carved → Tanker (peso alto) → grotesca condensada; Salted → outra script marcador; ADAM.CG → Tanker. Nunca degrade Atkinson (mantenha sempre, pela acessibilidade).

### 3.2 Hierarquia completa (escala relativa)

Escala modular ~1.25 (terça maior), base de corpo = 1rem (18px sugerido para leitura confortável).

| Nível | Família | Tamanho rel. | Peso / estilo | Uso |
|---|---|---|---|---|
| **Wordmark** | AW Conqueror Carved | 3.05–4.77rem+ | Carved inline | Só o logotipo "GRAVIDADE ZERO" e aberturas de parte. |
| **Display** | AW Conqueror Carved / Tanker | 2.44–3.05rem | Bold caps | Títulos de abertura, capas, heróis. No neon, ganha eco marquise. |
| **Título (H1)** | Salted | 1.95–2.44rem | Caixa-alta, baseline saltitante | Título de capítulo narrativo, headline afetivo. Sempre Rosa Spray (claro) / branco (neon). |
| **Seção (H2)** | Tanker | 1.56–1.95rem | Condensado bold caps | Rubricas de seção, sumário, "PRIMEIRA PARTE". |
| **Subtítulo (H3)** | Hepta Slab / Salted | 1.25–1.56rem | ExtraLight caps espaçado / manuscrito | Kickers, subheads, "com amor & spray rosa". |
| **Corpo** | Atkinson Hyperlegible | 1rem | Regular; Bold p/ ênfase; Italic p/ apartes | Todo texto corrido. Entrelinha 1.4–1.55, medida 40–58 caracteres. |
| **Legenda** | Atkinson / Hepta Slab | 0.8rem | Regular | Créditos, notas de rodapé, fólios, metadados. |
| **Código / máquina** | Menlo/Courier | 0.8–1rem | Regular | Blocos de código, "código-com-alma", CIP, glitch. |
| **Lettering / marginália** | Salted | 0.8–1.25rem | Manuscrito, rotação 90° | Voz do Bobo na margem (teal); pull-quote embutida (rosa). |

### 3.3 Tratamentos tipográficos característicos
- **Duplo registro voz oficial × voz do bobo:** Atkinson preto sério vs. Salted rosa/teal inclinado que comenta. Assinatura editorial central.
- **Promoção retórica:** a frase de maior peso é "promovida" do corpo preto para o lettering rosa à mão — vira âncora visual do parágrafo.
- **Carved com eco:** no Modo B, o título carved recebe linhas concêntricas em eco (tubo de neon) e sombra 3D listrada — "acende" sobre o preto.
- **Sumário sem líder de pontos:** o número de página vem em Preto colado ao fim do título Branco/rosa — o contraste de cor faz o papel da linha pontilhada.
- **Bloco de assinatura:** nome em Rosa Spray (Atkinson) + cargo abaixo em display condensado caps preto ("carimbo"). Assinatura da casa: **"RENANTE. SOMOS GZERO."** em Salted.
- **Zeros e detalhes:** o "0" recebe glifo especial (barra cortando `0̸` ou estrela de 8 pontas sobreposta) — device de marca no fólio e em números.
- **Aspas e parênteses desenhados à mão** dentro dos blocos de lettering.

---

## 4. GRID E LAYOUT

### 4.1 Sistema editorial (livros / PDF / páginas longas — Modo A)
- **Formato:** quadrado a levemente vertical (~1:1 a 1:1,08). Livro-objeto/artbook.
- **Coluna:** **única**, medida estreita **40–58 caracteres** (~50–60% da largura), **deslocada para a margem interna/centro**, deixando **margem externa larga (~25%) como calha de marginália**.
- **Alinhamento:** bandeira à esquerda (ragged-right) na prosa-poema; justificado só em prefácio/texto institucional; poesia sempre à esquerda.
- **Espaço em branco é premium:** fechos de capítulo usam 85–95% de vazio com texto curto no terço superior ou um único sketch de canto. O vazio é ritmo, não sobra.
- **Fólios:** numeral pequeno Atkinson, preto, no **canto externo** — **verso/par = inferior-esquerdo; recto/ímpar = superior-direito**. Diagramação espelhada. Ilustrações full-bleed e aberturas **não têm fólio**.
- **Molduras:** duas escolas convivem. Livro 1e2 = **sem moldura** (o enquadramento vem do vazio creme ou da cor chapada). Livro 3 = **moldura dupla de filete Rosa Spray** com cantoneiras art-déco/heráldicas, a ~6–8% da borda (cortina de proscênio / cercadura de decreto). Escolha uma por projeto e mantenha.
- **Ritmo "inspira/expira":** alterna spread ilustrado full-bleed ↔ páginas de texto claro ↔ páginas pretas/magenta de respiro.

### 4.2 Sistema de slides / bento (deck, social, cards — Modo B)
- **Formato:** 16:9 (slides), 1:1 e 4:5 (social), 9:16 (stories); ultra-wide para molduras.
- **Fundo:** Preto Palco `#080808`/`#0A0A0A` com specks sutis de ruído.
- **Collage-sticker:** elementos recortados (PNG alpha) sobrepostos como scrapbook; arte **sangra por uma ou duas bordas**; **bloco de texto no terço oposto**; muito espaço negativo no centro/topo-esquerda.
- **Bento:** grade **assimétrica** de cards de cantos muito arredondados ("adesivos"), ritmo de blocos grandes × pequenos, hierarquia por **saturação** (o magenta puxa o olho). Foto de produto encaixada no centro. Acabamento "editorial-punk / fanzine premium".
- **Sobreposição e diagonal:** composições diagonais ascendentes para "crescimento/decolagem"; simetria bilateral/radial nas cenas de palco (proscênio, mandala, sunburst).
- **Conectores:** linhas finas (amarelo-lima no neon, teal/seta no claro) amarram blocos e apontam relações.

### 4.3 Espaçamento (escala)
Escala base-4 / múltiplos de 8 para UI e slides: `2, 4, 8, 12, 16, 24, 32, 48, 64, 96, 128 px`. No editorial, o espaçamento é regido pela entrelinha do corpo (baseline ~1.5× corpo). Raio de canto: **sticker/bento = 16–24px**; chips/pills = total; molduras editoriais = 0 (cantos vivos vetoriais).

---

## 5. COMPONENTES RECORRENTES

Estes são os "tijolos" da marca. Cada um carrega o DNA e deve ser reutilizado com fidelidade.

- **Molduras de canto (cantoneiras):** colchetes/grampos art-déco, cartelas heráldicas ou **marcas de registro em "L"** nos cantos. Duas variantes: *decreto* (filigrana ornamental, miolo editorial) e *registro* (faixa chapada + keyline branca + marcas de corte, pranchas full-bleed). No neon a moldura **inverte para branca** sobre sangria magenta.
- **Fitas / banners ondulados:** faixa branca (ou contorno rosa) com nomes ou títulos, pontas recortadas em "boca de peixe", leve halftone. Usada para autoria na capa.
- **Balões de fala:** vazios, contorno rosa (ou duplo ondulado festonado no neon), interior reservado para texto. Motivo de "conversa".
- **Medalhas / selos circulares:** (a) **selo preto** sobre campo magenta com rótulo em arco ("•PRIMEIRA PARTE•") para abertura de parte; (b) **badge semicircular/disco magenta** com número de fábula vazado creme na base; (c) **orbe-selo** por dimensão (aro colorido à mão + spray + rótulo caps curvado no topo) — verde-lima=EMOCIONAL, roxo=CONTRATUAL, rosa=AFETIVO; (d) **medalhões** lua-crescente e estrela-de-8-pontas (par de capa).
- **Notas de margem (o componente mais distintivo):** bloco manuscrito **Salted em Teal**, **rotacionado 90°** (lê-se de baixo p/ cima) na calha externa, **sempre ligado à linha exata do corpo por uma seta curva desenhada à mão** (ponta em V aberto). Pode empilhar duas notas, cada uma com sua seta. A *persona* varia (Bobo irônico OU autor/epígrafe) — o tratamento visual é o mesmo; o teal é o **canal manuscrito de comentário lateral**.
- **Grifos marca-texto:** retângulo translúcido **Roxo Realce** (highlighter) sobre 1–3 palavras-chave por página — o "terceiro nível de anotação".
- **Assinatura "Renante":** lettering Salted rosa (claro) ou branco (neon) — **"RENANTE. SOMOS GZERO."** Fecho de manifesto e bloco de autoria.
- **Bloco de citação do Bobo da Corte (3 camadas):** (1) **ícone-mascote** (cabeça do Bobo em line-art rosa/branco) ancorando à margem; (2) **rubrica cênica** em Atkinson **Itálico rosa** ("*O Bobo da Corte entra pela porta da frente…*", "*Spoiler do Bobo:*"); (3) **fala** em **Salted caps** (rosa no claro / branco no neon), baseline dançante. A rubrica é opcional.
- **Logotipo GZERO:** "G" grande, ereto, grotesca pesada de cantos arredondados + "z-E-R-O" **tombando** (cada glifo girado num ângulo), **"O" final como quadrado arredondado (squircle)**. Duas texturas: chapada e rabiscada à mão. Sempre monocromático (branco knockout / preto).

### 5.1 Personagem-âncora: o Bobo da Corte
Um único personagem com **múltiplas fantasias** (não vários). Atributos fixos: **rosto redondo claro, olhos fechados sorridentes (ou um piscando), orelhas pontudas de elfo, bochechas coradas (blush halftone), gorro de bufão de 2–3 pontas com pompons/guizos, gola-rufo franzida, luvas brancas de cartoon (rubber-hose, 4 dedos)**. Figurinos variam (gorro gingham rosa, ou preto com poás amarelos, arlequim), a identidade não. Aparece em três escalas: **ícone-cabeça** (margem), **corpo inteiro** (pranchas), e **puro tipográfico/voz** (clímax neon). Renderiza em qualquer modo: line-art no claro, halftone/duotone no neon, pintura premium nas peças-herói. Outros motivos-mascote: **Coração Kawaii** (afeto), **Astronauta retrô** (guia do universo "zero-g"), **Sapo rosa** (merch), e o **robô-console ANI** (sequência de IA).

---

## 6. TEXTURAS E TRATAMENTOS

**Regra absoluta do sistema: NÃO existe gradiente digital suave.** Todo volume, sombra e gradação vem de **textura** — densidade de meio-tom ou hachura. Esta é a lei material da marca.

| Tratamento | O que é | Quando / como aplicar |
|---|---|---|
| **Halftone / meio-tom** | Retícula de pontos; densidade = valor (mais pontos = mais escuro). Variantes: redondo, xadrez/quadrado, losango, favo. | A textura-mãe. Sombreamento de personagens, fundos, blush, holofotes. **Nunca** substitua por gradiente. Em vetor, vira hachura. |
| **Riso / grão / misregistration** | Serigrafia/risografia de 2–4 tintas com **registro propositalmente frouxo**; overprint (magenta×amarelo→laranja-vermelho); respingos; grão de papel. | Todas as pranchas ilustradas. É o "acabamento impresso à mão". Deixe as bordas desalinhadas — não limpe. |
| **Spray / aerógrafo / stipple** | Névoa granulada de pontos. | Nuvens, glows, blush, bordas gastas de banner, pisos de palco, vinheta radial ("holofote invertido") atrás de lettering branco. |
| **Papel amassado / torn-paper / paper-craft** | Recorte de tesoura tosco, borda serrilhada, foil/mylar amassado, tiras de papel crepom. | Badges circulares, corações de foil, molduras de selo, colagem dadá. Bordas assumidamente ásperas. |
| **Duotone de fotos ("gzerização")** | Foto/gravura posterizada a 2 canais + grão riso. | Retratos, estátuas, gravuras de arquivo no Modo B. Receitas canônicas: **menta `#68F8A8` + magenta** (luz+sombra) ou **magenta + vinho `#3A0A2E`**. Sempre com film grain por cima. |
| **Crosshatch / gravura** | Hachura fina de buril, scratchboard, intaglio. | "Envelhecer"/costurar gravuras de domínio público ao traço neon; sombreado de vinco; a versão vetorial do meio-tom. |
| **Glow / bloom neon** | Halo emissivo, duplo-contorno, light-leak. | **Só no Modo B, só sobre preto.** Contornos tratados como luz, não como tinta. Jamais no editorial claro. |
| **Poema-fantasma** | O próprio texto reaparece translúcido, rotacionado, semi-apagado sobre a ilustração. | Marca-d'água/textura que amarra imagem e palavra. **Propositalmente ilegível** — não é para ser lido. |

**Contornos (dois idiomas, quase nunca misturados):** (a) **pincel/nanquim modulado** — pressão variável, tremor orgânico, terminais afilados/em gancho, dupla-passada visível; (b) **contorno branco grosso "de adesivo"** recortando massas de cor (as ilustrações leem como decalques colados). **O contorno colorido — rosa, lima ou roxo — no lugar do preto** é a assinatura mais forte do neon. Nunca vetor uniforme e limpo na arte autoral (a exceção é o subsistema de ícones de linha e a UI do produto).

---

## 7. DO'S & DON'TS

### ✅ DO — faça
1. **Comprometa-se com um modo por superfície.** Editorial claro OU neon escuro; alterne entre peças para criar ritmo, não dentro da mesma.
2. **Deixe o rosa liderar.** Se a peça não tem Rosa Spray como assinatura, provavelmente não parece Gzero.
3. **Use Preto Prensa `#231F20` (quente) para texto e fundos do Modo A** — nunca `#000000`.
4. **Dê ao corpo Atkinson entrelinha folgada (1.4–1.55) e medida curta (40–58 caracteres).** Legibilidade é valor de marca.
5. **Trate o vazio como premium.** Margens generosas, fechos arejados, calha externa reservada para marginália.
6. **Ancore a voz do Bobo na margem:** Salted teal, 90°, com seta curva à mão apontando a linha exata.
7. **Sombreie por textura** (halftone/hachura), sempre. Densidade = valor.
8. **Preserve o registro frouxo** do riso: overprint, respingo, borda desalinhada. A "imperfeição perfeita" é intencional.
9. **Contorne a arte neon com cor** (rosa/lima/roxo) e reserve o branco grosso de adesivo para recortar massas.
10. **Reserve os acentos neon (lima, menta, brasa) para o preto.** Sobre creme eles morrem.
11. **Use o duplo registro tipográfico:** texto sério + glosa manuscrita que comenta.
12. **Especifique Rosa Spray como spot color na impressão** e trate o "neon" como serigrafia 2–4 tintas.

### ❌ DON'T — não faça
1. **Não misture os dois modos na mesma superfície** (creme editorial com fundo preto de palco na mesma tela).
2. **Não use gradiente digital suave** como preenchimento ou sombra. Nunca.
3. **Não encoste Rosa Spray em Roxo Realce ou Teal sem contorno branco** — vibra e fica ilegível.
4. **Não use `#000000` puro no Modo A** nem trate o neon como se fosse tema dark de UI.
5. **Não aplique halftone, pincel ou glow em logos de terceiros** — eles entram sempre em knockout monocromático (branco/prata) sobre o preto.
6. **Não force o subsistema oliva (Humanware/Direito) ao magenta** da marca, nem o contrário.
7. **Não crave hex único para amarelos/vermelhos de ilustração** — são estimativas riso; não os use como cor de UI, texto ou fundo.
8. **Não limpe o traço** da arte autoral em vetor uniforme (exceto ícones de linha e UI de produto).
9. **Não transcreva o poema-fantasma** nem tente torná-lo legível — é textura, é ilegível de propósito.
10. **Não deforme o logotipo GZERO:** o "G" fica ereto, o "ZERO" tomba, o "O" final é squircle. Não alinhe tudo numa baseline reta.
11. **Não centralize colunas largas de corpo** — coluna estreita, ragged-left, deslocada à margem interna.
12. **Não trate o Bobo como personagens diferentes** — é um só, com fantasias variáveis; mantenha rosto redondo, olhos fechados, gorro de guizos, rufo, luvas.
13. **Não recrie marcas de terceiros por IA/vetor** — documente só o tratamento (knockout).
14. **Não empilhe glow/bloom no editorial claro** — brilho neon só existe sobre o preto do palco.

---

## 8. RESSALVAS E DIVERGÊNCIAS REGISTRADAS (não resolver silenciosamente)
- **Preto:** `#231F20` (editorial, quente) vs. `#080808`/`#000000` (fundo de palco neon). Ambos em uso, por modo.
- **Magenta neon ≠ magenta vetorial:** medições do deck dão neons mais quentes (`#E838A8`, `#EA33A6`) que `#EC008C`. O oficial (`#EC008C`) é a base; a família neon é acento do Modo B.
- **Verdes/menta/índigo/brasa:** fora da paleta vetorial oficial; canonizados aqui **apenas** como acentos do Modo B.
- **Persona da marginália teal:** ora Bobo irônico, ora autor/epígrafe (Schumacher, Botton, Fuller). Mesmo tratamento; conteúdo define a persona.
- **Estrela de 8 pontas** e **glifo do "0"** (barra vs. estrela): motivos de marca com variações de execução — trate como família, não engesse.
- **Balão de chat roxo** solto sobre arte: pode ser artefato de software (pin de comentário) — confirme na fonte antes de replicar; quando integrado à colagem, é design.
- **Subsistema oliva** e **paredes de logos de terceiros**: presentes no material mas **não são estilo autoral** de comunicação.

---

*Fim do documento. Tokens em `tokens.json` e `tokens.css`. "Com amor & spray rosa." — RENANTE. SOMOS GZERO.*
