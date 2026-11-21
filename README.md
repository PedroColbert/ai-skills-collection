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
