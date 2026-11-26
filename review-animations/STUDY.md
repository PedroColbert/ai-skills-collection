# review-animations — Study / Estudo

| | |
|---|---|
| **Source / Origem** | [emilkowalski/skills](https://github.com/emilkowalski/skills/tree/main/skills/review-animations) (MIT, ~60k ⭐, commit `64eb3de`) · [aiforui.dev/skills/review-animations](https://aiforui.dev/skills/review-animations) |
| **Area / Área** | Motion / Review |
| **Added / Adicionada** | 2026-11-25 |
| **Runs code? / Executa código?** | No — Markdown only (`SKILL.md` + `STANDARDS.md`) |

---

## 🇺🇸 English

**What it does.** Strict review of animation code against Emil's craft bar. Default is to flag; approval is earned.

**Manual only:** `disable-model-invocation: true` — Claude never picks it on its own; you start it by typing `/review-animations`.

**Core takeaways.**
- Ten non-negotiable standards: justified motion, frequency-appropriate, responsive easing (no `ease-in` on UI), sub-300ms UI, origin-aware (never `scale(0)`), interruptible, GPU-only properties, accessibility, asymmetric enter/exit, cohesion.
- Escalation triggers and a remedial preference hierarchy.
- Per-element budgets in `STANDARDS.md`.

**When to use.** Before merging motion work.

**When NOT to use.** Building new motion.

## 🇧🇷 Português

**O que faz.** Revisão rigorosa do código de animação pelos padrões do Emil. O padrão é apontar problemas; aprovação se conquista.

**Só manual:** `disable-model-invocation: true` — o Claude não usa sozinho; você inicia digitando `/review-animations`.

**Principais lições.**
- Dez padrões: animação justificada, adequada à frequência, `ease-out` (nunca `ease-in` em UI), menos de 300ms, origem correta, interrompível, só propriedades de GPU, acessível, entrada e saída assimétricas, coerente.

**Quando usar.** Antes de aprovar animações.

**Quando NÃO usar.** Criar animações.

---

## 🔗 Pairs with / Combina com
`improve-animations`, `animation-performance`

## 🧪 Used in / Usada em

_Not used in a project yet / Ainda não usada em projeto._
