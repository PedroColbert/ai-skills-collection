# animate — Study / Estudo

| | |
|---|---|
| **Source / Origem** | [emilkowalski/skills](https://github.com/emilkowalski/skills/tree/main/skills/animate) (MIT) |
| **Area / Área** | Motion |
| **Added / Adicionada** | 2026-11-15 (portfolio project) · collection 2026-11-21 |
| **Runs code? / Executa código?** | No |

---

## 🇺🇸 English

**What it does.** Builds one animation from scratch by making decisions in a fixed order: should it animate at all → purpose → cheapest tool → properties → easing/duration or spring → interruption & exit → reduced motion and hover gating. Writes the implementation.

**How it works.** `SKILL.md` holds the 7-step build sequence and hard rules; `RECIPES.md` has ready recipes with exact values.

**Core takeaways.**
- Steps 1–2 gate everything: many things should not animate.
- No invented curves: use the codebase's tokens or the skill's tables.
- Extend existing motion tokens, never fork a parallel system.
- Reduced motion and hover gating ship *with* the animation.
- Cheapest tool that works: don't install a library for a fade.

**When to use.** Adding a single transition, micro-interaction or entrance.

**When NOT to use.** Coordinating many elements at once (use `choreograph`).

## 🇧🇷 Português

**O que faz.** Cria uma animação do zero decidindo numa ordem fixa: deve animar? → propósito → ferramenta mais barata → propriedades → curva/duração ou mola → interrupção e saída → movimento reduzido.

**Principais lições.**
- Muita coisa não deve animar.
- Nada de curvas inventadas: usar os tokens do projeto.
- Movimento reduzido vem junto, não depois.
- Ferramenta mais simples que resolva.

**Quando usar.** Uma transição, micro-interação ou entrada.

**Quando NÃO usar.** Vários elementos coordenados (usar `choreograph`).

---

## 🔗 Pairs with / Combina com
`choreograph`, `emil-design-eng`, `better-ui`

## 🧪 Used in / Usada em

- **2026-11-15 — pedro-colbert-portfolio** (online CV site, Vite + TS + GSAP + React islands): installed as a project skill for the site's design and motion work.
- **2026-11-15 — pedro-colbert-portfolio** (currículo online, Vite + TS + GSAP + ilhas React): instalada como skill do projeto para o design e as animações do site.
