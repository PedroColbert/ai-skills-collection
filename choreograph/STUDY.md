# choreograph — Study / Estudo

| | |
|---|---|
| **Source / Origem** | [emilkowalski/skills](https://github.com/emilkowalski/skills/tree/main/skills/choreograph) (MIT) |
| **Area / Área** | Motion |
| **Added / Adicionada** | 2026-11-15 (portfolio project) · collection 2026-11-21 |
| **Runs code? / Executa código?** | No |

---

## 🇺🇸 English

**What it does.** Coordinates several elements that animate together (staggers, hero entrances, view swaps, multi-step flows) so the group reads as one intentional motion.

**How it works.** 5 steps: cast the elements → pick the relationship per pair (together / overlap / sequence) → sync secondary motion → adapt timing → direction and exits. Output is a timeline + what stays still + a feel check. `RECIPES.md` has patterns.

**Core takeaways.**
- One entrance per container: never animate the parent *and* stagger its children.
- No stagger on high-frequency or keyboard UI (menus, palettes, tabs).
- Uniform stagger is forbidden: vary timing by importance.
- Choreography never blocks interaction.
- Every sequence must survive interruption.

**When to use.** Hero entrances, staggered lists, crossfades, multi-part interactions.

**When NOT to use.** A single element (use `animate`).

## 🇧🇷 Português

**O que faz.** Coordena vários elementos animando juntos (stagger, entrada do hero, troca de telas) para o grupo parecer um movimento só.

**Principais lições.**
- Uma entrada por container.
- Sem stagger em interface usada toda hora.
- Stagger uniforme é proibido.
- A coreografia nunca bloqueia o clique.
- Tem que aguentar interrupção.

**Quando usar.** Entradas de hero, listas em sequência, transições com várias partes.

**Quando NÃO usar.** Um elemento só (usar `animate`).

---

## 🔗 Pairs with / Combina com
`animate`, `gsap-scrolltrigger`, `reanimate`

## 🧪 Used in / Usada em

- **2026-11-15 — pedro-colbert-portfolio** (online CV site, Vite + TS + GSAP + React islands): installed as a project skill for the site's design and motion work.
- **2026-11-15 — pedro-colbert-portfolio** (currículo online, Vite + TS + GSAP + ilhas React): instalada como skill do projeto para o design e as animações do site.
