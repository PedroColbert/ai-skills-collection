# jury — Study / Estudo

| | |
|---|---|
| **Source / Origem** | [juliobsz/skills](https://github.com/juliobsz/skills) (MIT, ~1.4K stars, commit `add880b`) |
| **Area / Área** | Web design QA |
| **Added / Adicionada** | 2026-11-23 |
| **Runs code? / Executa código?** | Yes — the same reviewed Node scripts as `awwwards` (`shoot.mjs`, `audit.mjs`, `serve.mjs`), needing Playwright + axe-core (installed in a cache folder, not in the project). |

---

## 🇺🇸 English

**What it does.** Scores any website the way an Awwwards jury would, from evidence only: screenshots (desktop, throttled phone, reduced motion, focus, hover), vitals, axe and an SEO audit, judged by a fresh critic that never sees the code.

**How it works.** Build/serve production → `shoot.mjs --crawl` + `audit.mjs` into `.jury/<host>/` → blind critic subagent scores Design, Usability, Creativity, Content and six developer areas → score card with evidence and a ranked fix list. Includes a calibration offset to estimate the real jury score.

**Core takeaways.** No evidence, no points; start each category at 6; never argue a score up; re-score with a new critic.

**When to use.** "Is this good enough for Awwwards?", pre-launch design QA, comparing two sites.

**When NOT to use.** Building or redesigning (use `awwwards`). Sites behind a login.

**⚠️ Caveats.** Scores are estimates, not affiliated with Awwwards. A self-score after building is not independent.

## 🇧🇷 Português

**O que faz.** Avalia qualquer site como um júri do Awwwards faria, só com evidências: screenshots (desktop, celular lento, movimento reduzido, foco, hover), métricas, axe e auditoria de SEO, julgados por um crítico novo que nunca vê o código.

**Como funciona.** Build de produção → `shoot.mjs --crawl` + `audit.mjs` em `.jury/<host>/` → subagente crítico cego dá notas de Design, Usabilidade, Criatividade, Conteúdo e seis áreas de dev → ficha com evidências e lista de correções priorizada.

**Principais lições.** Sem evidência, sem ponto; toda categoria começa em 6; nunca inflar nota; reavaliar com crítico novo.

**Quando usar.** "Isso está no nível Awwwards?", QA de design antes de publicar, comparar dois sites.

**Quando NÃO usar.** Para construir ou redesenhar (use `awwwards`). Sites atrás de login.

**⚠️ Cuidados.** As notas são estimativas, sem vínculo com o Awwwards. Autoavaliação depois de construir não é independente.

---

## 🔗 Pairs with / Combina com

`awwwards`, `web-design-guidelines`.

## 🧪 Used in / Usada em
