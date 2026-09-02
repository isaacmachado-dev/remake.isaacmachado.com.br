---
version: alpha
name: isaacmachado.com.br
description: Portfólio escuro e editorial para Isaac Machado — Full-Stack Developer. Atmosfera noturna com superfícies elevadas sutis e cartões claros como respiro.
colors:
  primary: "#100d1a"
  secondary: "#1b1820"
  tertiary: "#ffffff"
  neutral: "#d5d5d5"
  neutral-strong: "#d9d9d9"
  muted: "#969393"
  ink: "#0c0b0c"
  on-primary: "#ffffff"
  on-secondary: "#ffffff"
  on-tertiary: "#0c0b0c"
  on-neutral: "#0c0b0c"
typography:
  display:
    fontFamily: Inter
    fontSize: 4.5rem
    fontWeight: 700
    lineHeight: 1.2
    letterSpacing: "-0.03em"
  h1:
    fontFamily: Geist
    fontSize: 4rem
    fontWeight: 600
    lineHeight: 1.0
    letterSpacing: "-0.02em"
  h2:
    fontFamily: Geist
    fontSize: 2rem
    fontWeight: 700
    lineHeight: 1.0
  h3:
    fontFamily: "Gothic A1"
    fontSize: 3.125rem
    fontWeight: 700
    lineHeight: 1.0
  h4:
    fontFamily: "Gothic A1"
    fontSize: 2.5rem
    fontWeight: 700
    lineHeight: 1.0
  body-lg:
    fontFamily: Geist
    fontSize: 1.5rem
    fontWeight: 600
    lineHeight: 1.3
  body-md:
    fontFamily: Geist
    fontSize: 1rem
    fontWeight: 400
    lineHeight: 1.5
  label:
    fontFamily: Geist
    fontSize: 0.875rem
    fontWeight: 600
    lineHeight: 1.0
    letterSpacing: "0.08em"
  label-mono:
    fontFamily: "Geist Mono"
    fontSize: 1.5rem
    fontWeight: 600
    lineHeight: 1.0
    letterSpacing: "0.33em"
  logo:
    fontFamily: "Mea Culpa"
    fontSize: 3rem
    fontWeight: 400
    lineHeight: 1.0
  logo-sm:
    fontFamily: "Mea Culpa"
    fontSize: 2.5rem
    fontWeight: 400
    lineHeight: 1.0
rounded:
  sm: 12px
  md: 18px
  lg: 20px
  xl: 48px
  2xl: 66px
  pill: 70px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 48px
  2xl: 94px
  section: 1080px
components:
  button-primary:
    backgroundColor: "{colors.tertiary}"
    textColor: "{colors.on-tertiary}"
    rounded: "{rounded.sm}"
    padding: 12px
  button-primary-hover:
    backgroundColor: "{colors.neutral-strong}"
    textColor: "{colors.ink}"
  card:
    backgroundColor: "{colors.neutral}"
    textColor: "{colors.on-neutral}"
    rounded: "{rounded.md}"
    padding: 24px
  card-muted:
    backgroundColor: "{colors.muted}"
    textColor: "{colors.on-neutral}"
    rounded: "{rounded.md}"
    padding: 24px
  surface-elevated:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.on-secondary}"
    rounded: "{rounded.lg}"
    padding: 24px
  divider:
    backgroundColor: "{colors.neutral-strong}"
    textColor: "{colors.primary}"
    rounded: "{rounded.full}"
    height: 5px
  pill:
    backgroundColor: "{colors.neutral-strong}"
    textColor: "{colors.ink}"
    rounded: "{rounded.xl}"
    padding: 16px
---

## Overview

isaacmachado.com.br é um portfólio one-page em scroll vertical com narrativa editorial. Fundo dominante escuro (#100d1a) cria profundidade noturna; superfícies elevadas (#1b1820) aparecem como planos inclinados decorativos. Cartões claros (#d5d5d5 / #d9d9d9) interrompem o escuro para projetos e habilidades, e um bloco médio (#969393) ancora a seção de formação. Tipografia mistura Geist (UI e títulos), Inter Bold 72px para o hero, Gothic A1 para formação e Mea Culpa para o monograma "I/saac". O ritmo é dado por grandes números de seção (01/, 02/, 03/) e labels em caixa alta com tracking largo.

Figma: https://www.figma.com/design/FJ0lpj9PciSDFToSSLV0nc/isaacmachado.com.br?node-id=0-1&p=f — 6 frames: hero (1920x1080), experiencia, projetos (1920x1736), formacao, contato e footer. Draft exploratório com colagens também presente.

## Colors

- **Primary (#100d1a):** Fundo de página em todas as seções (hero, experiencia, projetos, formacao, contato). Quase preto com matiz violeta — base da identidade.
- **Secondary (#1b1820):** Superfície elevada decorativa — retângulo rotacionado de 31° no hero e bloco atrás de projetos. Um tom acima do primary para criar elevação sem sombra.
- **Tertiary (#ffffff):** Ação principal. Botão "Conversar comigo" (245x60, rounded 12px) usa fundo branco com texto #0c0b0c. Também cor de texto padrão sobre fundo escuro.
- **Neutral (#d5d5d5):** Cartão de projeto (930x351, rounded 18px) e cards de linguagens (156x137). Fundo claro para listar habilidades e projetos com texto preto.
- **Neutral-strong (#d9d9d9):** Divisor horizontal (5–6px, 1000px+), pill "2026" e texto do monograma "saac" no header. Variação levemente mais quente que neutral.
- **Muted (#969393):** Bloco 861x227 atrás de "Cursos" na formação — cinza médio que separa conteúdo sem competir com neutral.
- **Ink (#0c0b0c):** Texto sobre fundos claros e preenchimento do monograma "I" dentro da elipse. Preto quente, não puro #000.
- **On-primary / On-secondary (#ffffff):** Texto sobre fundos escuros. Contraste ~19:1 sobre primary.
- **On-tertiary / On-neutral (#0c0b0c):** Texto sobre fundos claros. Contraste ~19:1 sobre white e ~13:1 sobre #d5d5d5.

Uso: nunca aplicar neutral/muted como texto sobre escuro; reservar tertiary apenas para CTAs e texto de alto contraste.

## Typography

Escala extraída do Figma (Geist, Inter, Gothic A1, Geist Mono, Mea Culpa).

- **Display (Inter Bold 72px / 4.5rem, 700, 1.2, -0.03em):** "Full-Stak Developer" no hero (node 42:236, token SDS `Title Hero` — `var(--sds-typography-title-hero-size)` 72, Inter, 700). Letter-spacing -2.16px a -3px no Figma.
- **H1 (Geist SemiBold 64px / 4rem, 600, 1.0):** Títulos de seção — "Projetos", "Formação", "Contato" (nodes 42:276, 42:281, 42:286).
- **H2 (Geist Bold 32px / 2rem, 700):** Título de projeto dentro do card — "Parque dos Búfalos" (54:33).
- **H3 (Gothic A1 Bold 50px / 3.125rem, 700):** "Ensino superior" (51:30).
- **H4 (Gothic A1 Bold 40px / 2.5rem, 700):** "Cursos" (51:33). Variante Regular 32px para "UNIVESP" (51:31, Gothic A1 Regular 32px).
- **Body-lg (Geist SemiBold 24px / 1.5rem, 600):** Ações secundárias — "Quem eu sou?", "Visualizar proejtos", frases de formação/contato.
- **Body-md (Geist 16px, 400, 1.5):** Texto corrido padrão quando houver parágrafos.
- **Label (Geist SemiBold 14px / 0.875rem, 600, 0.08em):** Sistema de navegação editorial — "01/", "02/", "03/", "PRINCIPAIS HABILIDADES", "EXPERIÊNCIA COM", "CONTINUE". Sempre em caixa alta no Figma, branco sobre escuro.
- **Label-mono (Geist Mono SemiBold 24px, 600, 0.33em):** Citações de seção — "“O aluno quem faz é a escola”" e "Todo projeto começa com uma comunicação" (tracking 7.92px, shadow 0 4px 4px rgba(0,0,0,0.25)).
- **Logo (Mea Culpa Regular 48px / 3rem, 400):** "saac" no header (42:233); variante Logo-sm 40px para "I" dentro da elipse 60x56 (42:238, texto #0c0b0c sobre elipse clara).

Hierarquia: Display apenas uma vez por página (hero). H1 para cada dobra. Label para metadados de seção. Geist é a família de UI; Inter reservado ao hero; Gothic A1 à formação; Mea Culpa apenas ao monograma.

## Layout

Frames nativos 1920x1080 (hero, experiencia, formacao, contato) e 1920x1736 (projetos). Conteúdo alinhado em coluna com margens laterais ~82–174px (82px para "01/", 174px para títulos de seção). Espaçamento vertical entre seções é o próprio viewport (1080px de altura por dobra, scroll snap implícito).

- **Spacing xs 4px / sm 8px / md 16px / lg 24px / xl 48px:** Escala base 8px para gaps internos (padding de cards 24–33px observado).
- **2xl 94px:** Gap horizontal exato entre cards de linguagens (3 cards 156x137 por linha, 4 linhas em experiencia).
- **Section 1080px:** Altura de dobra — usar `min-h-[1080px]` ou `h-[100svh]` por seção no Astro.

Grid de linguagens: flex wrap com gap 94px, centralizado. Projetos: stack vertical com cards alternando offset horizontal (289px vs 233px/733px) — preservar desalinhamento intencional do Figma.

Imagem hero "2026 2" (744x1076, overflow hidden, object-cover 277% width) e plano rotacionado 31° por trás devem ser mantidos como camadas decorativas atrás do título.

## Elevation & Depth

Sem sombras projetadas no Figma. Profundidade vem de contraste de cor e rotação.

- **Camada 0:** Fundo primary #100d1a.
- **Camada 1:** Superfície secondary #1b1820 rotacionada (hero 31°, projetos sem rotação) — cria perspectiva sem blur.
- **Camada 2:** Cartões neutral #d5d5d5 elevados sobre ambas — cantos arredondados e cor clara bastam para separação.
- **Elementos flutuantes:** Vetores decorativos (Vector 1/2) e elipse 747x740 com opacidade baixa atrás de experiencia.

Evitar sombras; se necessário para acessibilidade em produção, usar `shadow-sm` sutil, nunca sombra forte.

## Shapes

- **sm 12px:** Botão primário "Conversar comigo".
- **md 18px:** Card de projeto (42:274) e card genérico.
- **lg 20px:** Cards de linguagens (rounded 19–20px nos nodes 42:244–246) — unificado em 20px.
- **xl 48px:** Pill vertical da timeline de formação (54:40, 212x96).
- **2xl 66px:** Bloco grande de contato (42:290, 1607x677, rounded 66px) — assinatura da seção final.
- **pill 70px:** Wrapper arredondado das linhas de linguagens (rounded 70px no container flex).
- **full 9999px:** Elipses do monograma e divisores finos se transformados em pílulas.

Divisores: 5px (projetos) e 6px (formacao/contato) de altura, largura 1000–1231px, cor #d9d9d9 — renderizar como `h-[5px] bg-neutral-strong`.

## Components

- **button-primary:** Fundo `{colors.tertiary}` branco, texto `{colors.on-tertiary}` #0c0b0c, `rounded: {rounded.sm}` 12px, padding 12px, font Geist SemiBold 24px. Usado para "Conversar comigo" (134,571, 245x60). Hover: `{colors.neutral-strong}` #d9d9d9 para feedback sutil mantendo texto ink.
- **button-primary-hover:** Variante sibling (não aninhada) — background #d9d9d9, mesmo texto e raio.
- **card:** Fundo `{colors.neutral}` #d5d5d5, texto `{colors.on-neutral}` #0c0b0c, rounded md 18px, padding 24px. Base para projetos e linguagens. Imagem interna 480x285 com `object-cover`.
- **card-muted:** Fundo `{colors.muted}` #969393, texto branco, mesmo raio/padding — para bloco "Cursos".
- **surface-elevated:** Fundo `{colors.secondary}` #1b1820, texto branco, rounded lg 20px — para planos decorativos atrás do hero/projetos.
- **divider:** Fundo `{colors.neutral-strong}` #d9d9d9, altura 5px, full width — linha editorial abaixo de títulos de seção.
- **pill:** Fundo `{colors.neutral-strong}`, texto ink, rounded xl 48px — timeline e badges de ano.

Variantes de hover/active devem ser entradas separadas (`button-primary-hover`), nunca objetos aninhados, conforme lint `broken-ref`.

## Do's and Don'ts

- **Do** manter o fundo global #100d1a em todas as dobras — a identidade é noturna. Não introduzir fundos claros como base.
- **Do** usar token references (`{colors.primary}`) nos componentes — paleta single-source.
- **Do** preservar o desalinhamento intencional dos cards de projetos e o plano rotacionado de 31° no hero — são gestos de design, não bugs de alinhamento.
- **Do** usar Geist para UI e reservar Inter apenas ao display do hero; não misturar Mea Culpa fora do monograma.
- **Do** manter labels 14px em caixa alta com tracking 0.08em para navegação editorial (01/, 02/, 03/).
- **Don't** adicionar cores além da paleta — se precisar de destaque, estender `colors` primeiro e referenciar.
- **Don't** aninhar variantes (`button.primary.hover`) — criar `button-primary-hover` como entrada irmã.
- **Don't** arredondar tudo em 8px — o Figma usa raios grandes e expressivos (18–66px); respeitar a escala `rounded`.
- **Don't** substituir o contraste branco-preto dos CTAs por cores de marca — o botão branco sobre dark é a assinatura de conversão.
