# 🧠 AI Skills Collection

> 🇧🇷 [Leia em português](README.pt-BR.md)

A living collection of **agent skills** for [Claude Code](https://claude.com/claude-code) that I study, document and actually use in my projects.

Each skill here is not just copied — it comes with a **study file (`STUDY.md`)** explaining what it does, when to use it, when *not* to use it, how it works under the hood and where I've applied it.

## 📚 What is a skill?

A skill is a folder with a `SKILL.md` file that teaches an AI agent a specialized workflow or domain knowledge (e.g. "how to design native Android UIs with Material 3"). The agent reads the skill's short description, and when a task matches, it loads the full instructions on demand.

```
skill-name/
├── SKILL.md        ← instructions the agent reads (name + description in frontmatter)
├── references/     ← optional deeper docs loaded only when needed
└── STUDY.md        ← my notes: what I learned about this skill (EN + PT)
```

This repository is cloned directly into `~/.claude/skills/`, so every skill here is **live** in all my Claude Code sessions.

## 🗂️ Skills

| Skill | Area | What it's for | Source |
|---|---|---|---|
| [find-skills](find-skills/STUDY.md) | Meta / tooling | Discover and install new skills from the open ecosystem | [vercel-labs/skills](https://github.com/vercel-labs/skills) |
| [mobile-android-design](mobile-android-design/STUDY.md) | Mobile UI | Material Design 3 + Jetpack Compose for native Android | [wshobson/agents](https://github.com/wshobson/agents) |
| [mobile-ios-design](mobile-ios-design/STUDY.md) | Mobile UI | Apple HIG + SwiftUI for native iOS/iPadOS | [wshobson/agents](https://github.com/wshobson/agents) |
| [reanimate](reanimate/STUDY.md) | Frontend / Motion | Clone any animation frame by frame and prove the copy moves the same | [NiazMorshed2007/reanimate](https://github.com/NiazMorshed2007/reanimate) |
| [animate](animate/STUDY.md) | Motion | Build one animation by deciding in the right order (should it animate? → easing → exit) | [emilkowalski/skills](https://github.com/emilkowalski/skills) |
| [choreograph](choreograph/STUDY.md) | Motion | Coordinate several elements so a group moves as one intentional motion | [emilkowalski/skills](https://github.com/emilkowalski/skills) |
| [gsap-scrolltrigger](gsap-scrolltrigger/STUDY.md) | Motion / GSAP | Official GSAP skill: scroll-linked animation, pinning, scrub | [greensock/gsap-skills](https://github.com/greensock/gsap-skills) |
| [gsap-plugins](gsap-plugins/STUDY.md) | Motion / GSAP | Official GSAP skill: SplitText, Flip, Draggable, MorphSVG… (all free) | [greensock/gsap-skills](https://github.com/greensock/gsap-skills) |
| [frontend-design](frontend-design/STUDY.md) | Web design | Distinctive visual direction that doesn't look templated | [anthropics/skills](https://github.com/anthropics/skills) |
| [build-awwwards-quality-sites](build-awwwards-quality-sites/STUDY.md) | Web design | Art-directed, motion-rich portfolio and landing sites | [MengTo/Skills](https://github.com/MengTo/Skills) |
| [awwwards](awwwards/STUDY.md) | Web design | Award-caliber sites from a one-line brief, with blind-critic QA loop | [juliobsz/skills](https://github.com/juliobsz/skills) |
| [jury](jury/STUDY.md) | Web design | Scores a site like an Awwwards jury, from screenshots and measurements | [juliobsz/skills](https://github.com/juliobsz/skills) |
| [ui-ux-pro-max](ui-ux-pro-max/STUDY.md) | UI/UX | Searchable local database of styles, palettes, fonts and UX rules | [nextlevelbuilder/ui-ux-pro-max-skill](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill) |
| [emil-design-eng](emil-design-eng/STUDY.md) | UI polish | Design-engineering details that make interfaces feel great | [emilkowalski/skills](https://github.com/emilkowalski/skills) |
| [better-ui](better-ui/STUDY.md) | UI polish | Exact values for radius, shadows, icons and motion | [jakubkrehel/skills](https://github.com/jakubkrehel/skills) |
| [better-colors](better-colors/STUDY.md) | Design system | Palettes as ramps, semantic tokens, measured contrast | [jakubkrehel/skills](https://github.com/jakubkrehel/skills) |
| [better-typography](better-typography/STUDY.md) | Typography | Type scale, spacing, font features, wrapping | [jakubkrehel/skills](https://github.com/jakubkrehel/skills) |
| [better-layout](better-layout/STUDY.md) | Layout | Grouping, alignment and layouts that survive resize, translation and RTL | [jakubkrehel/skills](https://github.com/jakubkrehel/skills) |
| [web-design-guidelines](web-design-guidelines/STUDY.md) | UI review | Audit UI code against Vercel's Web Interface Guidelines | [vercel-labs/agent-skills](https://github.com/vercel-labs/agent-skills) |
| [copywriting](copywriting/STUDY.md) | Content | Page copy with supportable claims and no AI tells | [coreyhaines31/marketingskills](https://github.com/coreyhaines31/marketingskills) |
| [animate-expo](animate-expo/STUDY.md) | Motion / React Native | Animation build sequence for Expo: Reanimated, gestures, haptics | [emilkowalski/skills](https://github.com/emilkowalski/skills) |
| [gestures](gestures/STUDY.md) | Motion | Drag, swipe and sheets that track the finger 1:1 and stay interruptible | [emilkowalski/skills](https://github.com/emilkowalski/skills) |
| [animation-performance](animation-performance/STUDY.md) | Motion / Performance | Find why animations drop frames; composite-only properties | [emilkowalski/skills](https://github.com/emilkowalski/skills) |
| [find-animation-opportunities](find-animation-opportunities/STUDY.md) | Motion / Audit | Read-only: where motion would help, and where it wouldn't | [emilkowalski/skills](https://github.com/emilkowalski/skills) |
| [remove-animations](remove-animations/STUDY.md) | Motion / Cleanup | Remove motion the interface doesn't need (only subtracts) | [emilkowalski/skills](https://github.com/emilkowalski/skills) |
| [improve-animations](improve-animations/STUDY.md) | Motion / Audit | Prioritised motion audit + self-contained plans for other agents | [emilkowalski/skills](https://github.com/emilkowalski/skills) |
| [review-animations](review-animations/STUDY.md) | Motion / Review | Strict review against 10 motion standards (`/review-animations`) | [emilkowalski/skills](https://github.com/emilkowalski/skills) |
| [animation-vocabulary](animation-vocabulary/STUDY.md) | Motion | Glossary: vague description → exact animation term | [emilkowalski/skills](https://github.com/emilkowalski/skills) |
| [apple-design](apple-design/STUDY.md) | Design principles | Apple's WWDC interface and fluid-motion principles, for the web | [emilkowalski/skills](https://github.com/emilkowalski/skills) |
| [mobile-native](mobile-native/STUDY.md) | Mobile web | Make a web app feel native on phones (100vh, zoom, sticky hover…) | [emilkowalski/skills](https://github.com/emilkowalski/skills) |
| [break-ui](break-ui/STUDY.md) | QA | Stress-test UI with worst-case data behind a dev-only toggle | [emilkowalski/skills](https://github.com/emilkowalski/skills) |
| [prototype](prototype/STUDY.md) | Design exploration | Several real variants behind a live picker (`/prototype`) | [emilkowalski/skills](https://github.com/emilkowalski/skills) |
| [learn-taste](learn-taste/STUDY.md) | Design memory | Turn a session's design corrections into rules in DESIGN.md (`/learn-taste`) | [emilkowalski/skills](https://github.com/emilkowalski/skills) |
| [pick-ui-library](pick-ui-library/STUDY.md) | Tooling | Curated library per frontend task (`/pick-ui-library`) | [emilkowalski/skills](https://github.com/emilkowalski/skills) |
| [ask-sonner](ask-sonner/STUDY.md) | Library guide | Guide to Sonner, the React toast library | [emilkowalski/skills](https://github.com/emilkowalski/skills) |
| [ask-emil](ask-emil/STUDY.md) | Router | Which Emil skill or sequence fits your situation (`/ask-emil`) | [emilkowalski/skills](https://github.com/emilkowalski/skills) |
| [write-swift](write-swift/STUDY.md) | Swift | Modern Swift: Swift 6 concurrency, value types, Swift Testing, macros | [emilkowalski/skills](https://github.com/emilkowalski/skills) |

## 📦 Studied, not installed

| Collection | What it is | Notes |
|---|---|---|
| [ECC — Everything Claude Code](_studies/ecc/STUDY.md) | Agent-harness toolkit: 328 skills, 72 agents, hooks, rules, memory | Analysed for fit and risk; key ideas and cherry-pick list documented |

➡️ Full details, use cases and combinations: **[CATALOG.md](CATALOG.md)**

## 🔁 How this repo grows

1. I find an interesting skill while studying.
2. It gets reviewed (content + any scripts it runs), installed and documented in a `STUDY.md`.
3. Whenever a skill is used in a real project, the project is added to its **"Used in"** section.

## ⚖️ Credits & licenses

Third-party skills keep their original authors and licenses — see [THIRD_PARTY.md](THIRD_PARTY.md). My own notes and skills are under the [MIT License](LICENSE).
