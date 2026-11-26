# break-ui — Study / Estudo

| | |
|---|---|
| **Source / Origem** | [emilkowalski/skills](https://github.com/emilkowalski/skills/tree/main/skills/break-ui) (MIT, ~60k ⭐, commit `64eb3de`) · [aiforui.dev/skills/break-ui](https://aiforui.dev/skills/break-ui) |
| **Area / Área** | QA / Robustness |
| **Added / Adicionada** | 2026-11-25 |
| **Runs code? / Executa código?** | No — Markdown only (`SKILL.md` + `CATALOG.md` (worst-case data catalog)) |

---

## 🇺🇸 English

**What it does.** Tries to break a UI with worst-case data (long names, unbreakable emails, one-letter names, huge counts, empty lists, non-Latin text, emoji) behind a dev-only "Demo / Worst case" toggle, then reports every break with a fix.

**Core takeaways.**
- Plausible or schema-backed values, never random.
- Change the data, not the component.
- One dataset hits every failure at once.
- The toggle never ships to production.
- Report before fixing — some breaks are design decisions.

**When to use.** Before shipping cards, tables, profiles, lists.

**When NOT to use.** Purely static marketing copy you control.

## 🇧🇷 Português

**O que faz.** Tenta quebrar a interface com dados extremos (nomes enormes, e-mails sem quebra, listas vazias, emoji, textos não latinos) atrás de um botão só de desenvolvimento, e relata cada falha com a correção.

**Principais lições.**
- Valores realistas ou do schema, nunca aleatórios.
- Mudar os dados, não o componente.
- Relatar antes de corrigir.

**Quando usar.** Antes de publicar cards, tabelas, perfis, listas.

**Quando NÃO usar.** Texto fixo que você controla.

---

## 🔗 Pairs with / Combina com
`better-layout`, `better-typography`, `jury`

## 🧪 Used in / Usada em

_Not used in a project yet / Ainda não usada em projeto._
