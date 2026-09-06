# Hero — `src/components/hero/`

## Estrutura
- `Hero.astro`: header monograma + `section` hero 1920x1080 (`min-h-svh`, `bg-primary`).
- Camadas: `0` fundo `primary #100d1a`, `1` plano `secondary #1b1820` com `.hero-tilt rotate(31.07deg)`, `2` conteúdo + foto `744x1076 object-cover`.
- Tokens: `Display Inter 72px 700 -0.03em` só no `h1`, `Label 14px 0.08em uppercase` para `01/`, `body-lg 24px 600` nos CTAs, `button-primary 12px white/ink → hover neutral-strong`, `rounded sm 12px / lg 20px`.

## Por que
- Single-source via `@theme` em `global.css`; sem sombra, profundidade por contraste + rotação (cf. `docs/DESIGN.md`).
- `astro:assets Image` com `width/height` fixos evita CLS; `overflow-hidden` recorta foto como no Figma `2026 2`.
- Links âncora `#contato` / `#projetos` preparam scroll para próximas dobras.
