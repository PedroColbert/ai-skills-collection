# ui-ux-pro-max — Study / Estudo

| | |
|---|---|
| **Source / Origem** | [nextlevelbuilder/ui-ux-pro-max-skill](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill/tree/main/.claude/skills/ui-ux-pro-max) (MIT) |
| **Area / Área** | UI/UX knowledge base |
| **Added / Adicionada** | 2026-11-15 (portfolio project) · collection 2026-11-21 |
| **Runs code? / Executa código?** | Yes — Python 3 search scripts (stdlib only, offline) |

---

## 🇺🇸 English

**What it does.** UI/UX design intelligence backed by a **local searchable database**: 80 styles, 192 product palettes & reasoning profiles, 74 font pairings, 120 UX guidelines, icons, 17 GSAP presets, 25 chart types, 22 stacks.

**How it works.** `scripts/search.py "<query>" --domain <domain>` searches 37 CSV files; `--design-system` generates a full design system and `--persist` writes `design-system/MASTER.md` (+ page overrides) into the project. Includes `references/`, data provenance and a test suite.

**Core takeaways.**
- Workflow: analyse requirements → generate a design system (required for new pages) → supplementary searches → stack guidelines.
- Master + overrides pattern: page files override `MASTER.md`; `--persist` won't overwrite an existing master without `--force`.
- Optional "design dials" to tune the result.
- Run the script by its full path inside the skill; try `python`, `python3`, then `py -3`.

**When to use.** Starting a design system, choosing palettes/fonts/styles for a product type, stack-specific UI rules.

**When NOT to use.** When the visual direction is already decided (as in the portfolio).

**⚠️ Caveats.** Largest skill in the collection (~3.7 MB of CSV/JSON data). Safety review 2026-11-21: Python stdlib only, no network, writes only `design-system/` when `--persist` is passed.

## 🇧🇷 Português

**O que faz.** Base de conhecimento de UI/UX com **banco de dados local pesquisável**: estilos, paletas por tipo de produto, pares de fontes, regras de UX, presets de GSAP, tipos de gráfico e 22 stacks.

**Principais lições.**
- Fluxo: entender o pedido → gerar o design system → buscas extras → regras da stack.
- Padrão master + sobrescritas por página.
- Scripts em Python puro, sem internet.

**Quando usar.** Começar um design system, escolher paleta e fontes.

**Quando NÃO usar.** Quando a direção visual já está decidida.

**⚠️ Cuidados.** Maior skill da coleção (~3,7 MB de dados). Revisão de segurança em 2026-11-21: só biblioteca padrão do Python, sem rede; só escreve `design-system/` com `--persist`.

---

## 🔗 Pairs with / Combina com
`better-colors`, `better-typography`, `frontend-design`

## 🧪 Used in / Usada em

- **2026-11-15 — pedro-colbert-portfolio** (online CV site, Vite + TS + GSAP + React islands): installed as a project skill for the site's design and motion work.
- **2026-11-15 — pedro-colbert-portfolio** (currículo online, Vite + TS + GSAP + ilhas React): instalada como skill do projeto para o design e as animações do site.
