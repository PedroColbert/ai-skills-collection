# animation-performance — Study / Estudo

| | |
|---|---|
| **Source / Origem** | [emilkowalski/skills](https://github.com/emilkowalski/skills/tree/main/skills/animation-performance) (MIT, ~60k ⭐, commit `64eb3de`) · [aiforui.dev/skills/animation-performance](https://aiforui.dev/skills/animation-performance) |
| **Area / Área** | Motion / Performance |
| **Added / Adicionada** | 2026-11-25 |
| **Runs code? / Executa código?** | No — Markdown only (`SKILL.md`) |

---

## 🇺🇸 English

**What it does.** Keeps web animations inside the frame budget and diagnoses jank: which properties to animate, where the animation runs (compositor vs main thread), and why it drops frames.

**Core takeaways.**
- `transform` and `opacity` by default; anything else needs a reason.
- Name the cause before changing code — "added will-change, seems smoother" is not a diagnosis.
- Never `transition: all`.
- React: don't animate through state (re-render per frame).
- Never conclude "it's fine" from a fast machine.

**When to use.** Janky, stuttering animations; choosing CSS vs JS vs WAAPI.

**When NOT to use.** Deciding *whether* to animate (use `animate` / `remove-animations`).

## 🇧🇷 Português

**O que faz.** Mantém as animações web dentro do orçamento de quadros e descobre por que uma animação engasga.

**Principais lições.**
- Animar `transform` e `opacity` por padrão.
- Dar nome à causa antes de mexer no código.
- Nunca `transition: all`.
- Não concluir que está bom testando num computador rápido.

**Quando usar.** Animações travando; escolher entre CSS e JS.

**Quando NÃO usar.** Decidir se algo deve animar.

---

## 🔗 Pairs with / Combina com
`reanimate`, `review-animations`

## 🧪 Used in / Usada em

_Not used in a project yet / Ainda não usada em projeto._
