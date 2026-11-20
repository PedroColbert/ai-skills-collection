# mobile-ios-design — Study / Estudo

| | |
|---|---|
| **Source / Origem** | [wshobson/agents → plugins/ui-design](https://github.com/wshobson/agents/tree/main/plugins/ui-design/skills/mobile-ios-design) (MIT, ~42k ⭐) |
| **Area / Área** | Mobile UI — iOS / iPadOS |
| **Added / Adicionada** | 2026-11-14 |
| **Runs code? / Executa código?** | No — knowledge only / Não, só conhecimento |

---

## 🇺🇸 English

**What it does.** Teaches the agent Apple's **Human Interface Guidelines (HIG)** and modern **SwiftUI** patterns so generated apps feel native on iPhone and iPad.

**Structure.**
- `SKILL.md` — HIG principles, layout system, navigation, system integration, visual design, quick-start card, best practices.
- `references/hig-patterns.md`, `references/swiftui-components.md`, `references/ios-navigation.md` — deeper material loaded on demand.

**Core takeaways.**
- HIG pillars: **Clarity, Deference, Depth**.
- Layout: `VStack`/`HStack`, `LazyVGrid` with `.adaptive` columns.
- Navigation: `NavigationStack` + `navigationDestination` (iOS 16+), new `Tab` API in `TabView` (iOS 18+). Link values must be `Hashable`.
- **SF Symbols** with rendering modes, variable values and `.symbolEffect` (iOS 17+).
- **Dynamic Type**: semantic fonts (`.body`, `.headline`), `relativeTo:` for custom fonts.
- Semantic colors (`.primary`, `.secondary`) and materials (`.ultraThinMaterial`) → automatic dark mode.
- Accessibility labels/hints, safe areas, `@SceneStorage` for state restoration, iPad multitasking.
- Test on a real device (haptics/performance).

**When to use.** SwiftUI apps, iOS UI reviews, adapting an app to iPad.

**When NOT to use.** UIKit-only legacy codebases or cross-platform frameworks.

## 🇧🇷 Português

**O que faz.** Ensina ao agente as **Human Interface Guidelines (HIG)** da Apple e padrões modernos de **SwiftUI**, para que os apps pareçam nativos no iPhone e no iPad.

**Principais lições.**
- Pilares do HIG: **Clareza, Deferência, Profundidade**.
- Layout com stacks e grids adaptativos.
- Navegação com `NavigationStack` (iOS 16+) e a nova API `Tab` (iOS 18+).
- **SF Symbols**, **Dynamic Type** e cores semânticas → acessibilidade e modo escuro de graça.
- Rótulos de acessibilidade, safe areas, restauração de estado e multitarefa no iPad.
- Testar em aparelho real.

**Quando usar.** Apps SwiftUI, revisão de UI iOS, adaptar app para iPad.

**Quando NÃO usar.** Código legado só em UIKit ou frameworks multiplataforma.

---

## 🔗 Pairs with / Combina com
`mobile-android-design`.

## 🧪 Used in / Usada em

_Not used in a project yet / Ainda não usada em projeto._
