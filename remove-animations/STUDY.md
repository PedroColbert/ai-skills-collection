# remove-animations — Study / Estudo

| | |
|---|---|
| **Source / Origem** | [emilkowalski/skills](https://github.com/emilkowalski/skills/tree/main/skills/remove-animations) (MIT, ~60k ⭐, commit `64eb3de`) · [aiforui.dev/skills/remove-animations](https://aiforui.dev/skills/remove-animations) |
| **Area / Área** | Motion / Cleanup |
| **Added / Adicionada** | 2026-11-25 |
| **Runs code? / Executa código?** | No — Markdown only (`SKILL.md`) |

---

## 🇺🇸 English

**What it does.** Finds animations an interface doesn't need (keyboard actions, high-frequency surfaces, functional data, decoration) and removes them, cleaning up what they leave behind. Only subtracts.

**Core takeaways.**
- Only subtract — never add or retune motion.
- Check what depends on an animation before deleting it (visibility, unmount timing).
- Ask before uninstalling a motion library.
- Respect documented decisions.

**When to use.** "The app feels slow", "too much animation" — e.g. fade-ins on every section.

**When NOT to use.** Adding motion.

## 🇧🇷 Português

**O que faz.** Encontra e remove animações desnecessárias (atalhos de teclado, telas usadas toda hora, fade-in em toda seção) e limpa o que sobrar. Só subtrai.

**Principais lições.**
- Só remove, nunca adiciona.
- Verificar dependências antes de apagar.
- Perguntar antes de desinstalar biblioteca.

**Quando usar.** "O app parece lento", "animação demais".

**Quando NÃO usar.** Adicionar animação.

---

## 🔗 Pairs with / Combina com
`find-animation-opportunities` (the opposite), `review-animations`

## 🧪 Used in / Usada em

_Not used in a project yet / Ainda não usada em projeto._
