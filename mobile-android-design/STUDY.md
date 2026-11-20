# mobile-android-design — Study / Estudo

| | |
|---|---|
| **Source / Origem** | [wshobson/agents → plugins/ui-design](https://github.com/wshobson/agents/tree/main/plugins/ui-design/skills/mobile-android-design) (MIT, ~42k ⭐) |
| **Area / Área** | Mobile UI — Android |
| **Added / Adicionada** | 2026-11-14 |
| **Runs code? / Executa código?** | No — knowledge only / Não, só conhecimento |

---

## 🇺🇸 English

**What it does.** Gives the agent a solid playbook for **native Android UI** with **Material Design 3 (Material You)** and **Jetpack Compose**: components, theming, navigation and adaptive layouts.

**Structure.**
- `SKILL.md` — when to use, a quick-start Compose component (list card), best practices and common pitfalls.
- `references/details.md` — core concepts (moved out of SKILL.md to respect an 8 KB body limit).
- `references/compose-components.md` — Compose component patterns.
- `references/material3-theming.md` — color schemes, dynamic color, typography, shapes.
- `references/android-navigation.md` — Navigation Compose, back handling, deep links.

This is **progressive disclosure**: the short SKILL.md is loaded first, references only when the task needs them — it saves context.

**Core takeaways.**
- Read colors from `MaterialTheme.colorScheme` → free dark mode.
- Enable **dynamic color** on Android 12+.
- Use `WindowSizeClass` for phones / tablets / foldables.
- 48dp minimum touch targets; `contentDescription` on interactive elements.
- **State hoisting**; `remember` vs `rememberSaveable` (survives rotation).
- `LazyColumn` for long lists; avoid unstable lambdas (recomposition).
- `@Preview` with multiple configurations.

**When to use.** Kotlin + Compose apps, Android UI reviews, migrating XML views to Compose.

**When NOT to use.** Flutter / React Native / web — only the Material principles transfer.

## 🇧🇷 Português

**O que faz.** Dá ao agente um guia sólido de **UI Android nativa** com **Material Design 3 (Material You)** e **Jetpack Compose**: componentes, temas, navegação e layouts adaptativos.

**Estrutura.** `SKILL.md` curto + pasta `references/` com detalhes (componentes, tema M3, navegação). É **divulgação progressiva**: o agente só carrega as referências quando precisa, economizando contexto.

**Principais lições.**
- Cores via `MaterialTheme.colorScheme` → modo escuro automático.
- **Cores dinâmicas** no Android 12+.
- `WindowSizeClass` para celular / tablet / dobráveis.
- Alvos de toque de no mínimo 48dp; `contentDescription` nos elementos interativos.
- **Elevar o estado** (state hoisting); `remember` vs `rememberSaveable` (sobrevive à rotação).
- `LazyColumn` em listas longas; evitar lambdas instáveis (recomposição).

**Quando usar.** Apps Kotlin + Compose, revisão de UI Android, migração de XML para Compose.

**Quando NÃO usar.** Flutter / React Native / web — só os princípios do Material se aplicam.

---

## 🔗 Pairs with / Combina com
`mobile-ios-design` — same product on both platforms / mesmo produto nas duas plataformas.

## 🧪 Used in / Usada em

_Not used in a project yet / Ainda não usada em projeto._
