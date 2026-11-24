# better-ui — Study / Estudo

| | |
|---|---|
| **Source / Origem** | [jakubkrehel/skills](https://github.com/jakubkrehel/skills/tree/main/skills/better-ui) (MIT) |
| **Area / Área** | UI polish |
| **Added / Adicionada** | 2026-11-15 (portfolio project) · collection 2026-11-21 |
| **Runs code? / Executa código?** | No |

---

## 🇺🇸 English

**What it does.** Polishes surfaces, icons and motion with exact values: border radius, optical alignment, shadows, icon states and animation.

**How it works.** `SKILL.md` + references: animations, enter/exit, icon transitions, icons, performance, surfaces.

**Core takeaways.**
- Outer radius = inner radius + padding.
- Shadows for elevation, borders for structure.
- Press scales to 0.96; high-frequency interactions respond instantly.
- Exits shorter and smaller than enters; stagger infrequent entrances by 100ms.
- Suppress transitions on theme switch; hover effects only on hover-capable pointers.

**When to use.** Final polish pass on components and pages.

**When NOT to use.** Choosing the overall visual direction.

## 🇧🇷 Português

**O que faz.** Dá acabamento a superfícies, ícones e animações com valores exatos: raio de borda, alinhamento óptico, sombras, estados de ícones.

**Principais lições.**
- Raio externo = raio interno + padding.
- Sombra para elevação, borda para estrutura.
- Saídas menores e mais curtas que entradas.
- Desligar transições ao trocar de tema.

**Quando usar.** Passada final de acabamento.

**Quando NÃO usar.** Escolher a direção visual.

---

## 🔗 Pairs with / Combina com
`emil-design-eng`, `better-colors`

## 🧪 Used in / Usada em

- **2026-11-15 — pedro-colbert-portfolio** (online CV site, Vite + TS + GSAP + React islands): installed as a project skill for the site's design and motion work.
- **2026-11-15 — pedro-colbert-portfolio** (currículo online, Vite + TS + GSAP + ilhas React): instalada como skill do projeto para o design e as animações do site.
- **2026-11-24 — alessandra-colbert-portfolio**: swapped depth-only borders for layered shadows (with a transparent border for forced colors), added the 0.96 press scale behind reduced-motion, and applied the theme-switch transition suppression so the light/dark toggle stops smearing.
- **2026-11-24 — alessandra-colbert-portfolio**: trocou bordas que só davam profundidade por sombras em camadas (com borda transparente para o modo de alto contraste), adicionou o aperto de 0,96 nos botões respeitando o movimento reduzido e aplicou a supressão de transições na troca de tema, que deixou de "borrar" no claro/escuro.
