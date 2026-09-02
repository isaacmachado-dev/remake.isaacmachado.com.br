# AGENTS.md — www.v2-isaacmachado.com.br

## Stack
- Astro 7.2 + ESM (`"type": "module"`), Node `>=22.12.0` (see `package.json:6`)
- Strict TS via `astro/tsconfigs/strict` (`tsconfig.json:2`), `.astro/` is generated types — do not edit
- `astro.config.mjs:5` is empty `defineConfig({})` — add integrations there
- Single-page portfolio; no test/lint/CI configured yet

## Commands
- `npm install` — install
- `npm run dev` — dev at `localhost:4321`; for background use `npx astro dev --background` then `npx astro dev status|logs|stop`
- `npm run build` → `dist/` (ignored), `npm run preview` — verify production build
- `npm run astro -- --help` / `npm run astro -- check` — Astro CLI passthrough (`.vscode/launch.json:5` also launches `astro dev`)

## Project Structure
- `src/pages/index.astro:1` — only route (`/`); Astro file-based routing, `.astro`/`.md` in `src/pages/` become routes
- `src/pages/index.astro:2` uses `astro:assets` (`Image`) — prefer `src/assets/` for optimized images, `public/` for static passthrough (favicons currently in `public/`)
- `public/` — static assets copied verbatim; `dist/` and `.astro/` are build/generational artifacts (see `.gitignore:2`)

## Design System — read before styling
- Source of truth: `docs/DESIGN.md` — colors, typography, spacing, radii, and component specs extracted from Figma (6 frames, 1920x1080). Do not invent tokens.
- Palette: `primary #100d1a` (page bg), `secondary #1b1820` (elevated rotated plane 31°), `tertiary #ffffff` (CTA), `neutral #d5d5d5` / `neutral-strong #d9d9d9` (cards/dividers), `muted #969393`, `ink #0c0b0c`. Use `{colors.*}` references.
- Typography `docs/DESIGN.md:17`: Display Inter 72px (hero only), H1-H4 Geist/Gothic A1, Label 14px uppercase `0.08em`, Mono 24px `0.33em`, Logo Mea Culpa. Geist = UI default.
- Do: keep global dark bg, preserve intentional mis-aligned project cards and 31° hero plane, use large radii `12–66px` (`docs/DESIGN.md:77`), never nest variants (`button-primary-hover` as sibling — `docs/DESIGN.md:211`).
- Figma: https://www.figma.com/design/FJ0lpj9PciSDFToSSLV0nc/isaacmachado.com.br?node-id=0-1&p=f

## Gotchas
- No `opencode.json`, no `.github/workflows` — no codegen/migration steps to run
- Repo locale is `pt-BR` in docs/design, default `index.astro:5` `lang="en"` — update when building real content
- VS Code extension: `astro-build.astro-vscode` recommended (`.vscode/extensions.json:2`)
