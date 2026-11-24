# awwwards — Study / Estudo

| | |
|---|---|
| **Source / Origem** | [juliobsz/skills](https://github.com/juliobsz/skills) (MIT, ~1.4K stars, commit `add880b`) |
| **Area / Área** | Web design / motion |
| **Added / Adicionada** | 2026-11-23 |
| **Runs code? / Executa código?** | Yes — optional Node 20+ scripts: `shoot.mjs` (Playwright screenshots, vitals, axe, keyboard, hover), `audit.mjs` (SEO/meta/a11y audit), `font.mjs` (downloads Google/Fontshare fonts), `photos.mjs` (picsum placeholder photos), `og.mjs`, `serve.mjs`. Reviewed: network only to font CDNs, picsum and jsdelivr (axe with SRI hash); writes only to its output folders. |

---

## 🇺🇸 English

**What it does.** Turns a one-line brief into a finished, award-caliber site, using Awwwards' public scoring (Design 40, Usability 30, Creativity 20, Content 10 + developer review) as the quality bar.

**How it works.** Phased workflow: Brief → three concepts from different territories, scored → art-direction system written to `DESIGN.md` (palette, type, grid, motion verb, ASCII wireframes) → build (GSAP + Lenis engine, one clock, data-attribute API) → QA loop with screenshots, audit and a blind critic subagent until every category scores ≥ 8 → ship.

**Core takeaways.** One point of view taken from the subject's own world; every static frame is a poster; one signature moment; continuous motion between states; usability is 30% of the score; real content, no invented credentials.

**When to use.** Portfolios, personal and studio sites, launches, landing pages that must impress.

**When NOT to use.** Dashboards and app UIs. For a quick review without changes use `jury`.

**⚠️ Caveats.** Defaults to Next.js/Astro scaffolds; in an existing static site port only the pieces you need. Screenshot QA needs Playwright + Chromium.

## 🇧🇷 Português

**O que faz.** Transforma um briefing de uma linha em um site completo nível "prêmio", usando a pontuação pública do Awwwards (Design 40, Usabilidade 30, Criatividade 20, Conteúdo 10 + revisão de dev) como régua.

**Como funciona.** Fases: briefing → três conceitos de territórios diferentes, pontuados → sistema de direção de arte em `DESIGN.md` → construção (motor GSAP + Lenis, um único relógio) → ciclo de QA com screenshots, auditoria e um crítico cego (subagente) até todas as notas ≥ 8 → publicação.

**Principais lições.** Um ponto de vista tirado do mundo do próprio assunto; cada quadro parado é um pôster; um momento-assinatura; movimento contínuo entre estados; usabilidade vale 30%; conteúdo real, sem credenciais inventadas.

**Quando usar.** Portfólios, sites pessoais e de estúdio, lançamentos, landing pages que precisam impressionar.

**Quando NÃO usar.** Dashboards e interfaces de app. Para só avaliar, use `jury`.

**⚠️ Cuidados.** O padrão é Next.js/Astro; num site estático existente, porte só as peças necessárias. O QA por screenshots precisa de Playwright + Chromium.

---

## 🔗 Pairs with / Combina com

`jury`, `gsap-scrolltrigger`, `gsap-plugins`, `build-awwwards-quality-sites`, `frontend-design`, `emil-design-eng`.

## 🧪 Used in / Usada em

- **2026-11-23 — alessandra-colbert-portfolio** (static GitHub Pages site for an early childhood teacher): ran the concept phase (watercolor bloom chosen over two alternatives), wrote `DESIGN.md`, ported a minimal GSAP + Lenis engine to vanilla JS, self-hosted fonts with `font.mjs`, generated the OG image with `og.mjs` and used `audit.mjs` to fix accessible names, meta length and image weight.
- **2026-11-23 — alessandra-colbert-portfolio** (site estático no GitHub Pages de uma professora de Educação Infantil): fez a fase de conceito (aquarela que floresce, escolhida entre três), escreveu o `DESIGN.md`, portou um motor GSAP + Lenis mínimo para JS puro, hospedou fontes com `font.mjs`, gerou a imagem OG com `og.mjs` e usou o `audit.mjs` para corrigir nomes acessíveis, tamanho da descrição e peso das imagens.
