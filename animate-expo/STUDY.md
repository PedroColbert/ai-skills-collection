# animate-expo — Study / Estudo

| | |
|---|---|
| **Source / Origem** | [emilkowalski/skills](https://github.com/emilkowalski/skills/tree/main/skills/animate-expo) (MIT, ~60k ⭐, commit `64eb3de`) · [aiforui.dev/skills/animate-expo](https://aiforui.dev/skills/animate-expo) |
| **Area / Área** | Motion / React Native |
| **Added / Adicionada** | 2026-11-25 |
| **Runs code? / Executa código?** | No — Markdown only (`SKILL.md` + `RECIPES.md`) |

---

## 🇺🇸 English

**What it does.** The `animate` build sequence for **React Native and Expo**: should it animate → which thread → properties → spring or timing → gesture hand-off → degradation. Writes code with Reanimated, Gesture Handler, Expo Router and haptics.

**Core takeaways.**
- Reanimated, not core `Animated`: gesture logic must run on the UI thread (worklets).
- Install through `npx expo install` so versions match the SDK.
- Covers setup that silently breaks motion and 120fps (ProMotion) details.
- Feel is only verified on a **release build** on the slowest supported device.

**When to use.** Animations, sheets and gestures in an Expo/React Native app.

**When NOT to use.** Web projects (use `animate`).

## 🇧🇷 Português

**O que faz.** A sequência do `animate` para **React Native e Expo**, com Reanimated, Gesture Handler, Expo Router e vibração (haptics).

**Principais lições.**
- Reanimated em vez do `Animated` padrão.
- Instalar com `npx expo install`.
- Só vale testar em build de produção no aparelho mais lento.

**Quando usar.** Animações e gestos em apps Expo/React Native.

**Quando NÃO usar.** Projetos web.

---

## 🔗 Pairs with / Combina com
`gestures`, `apple-design`, `mobile-android-design`, `mobile-ios-design`

## 🧪 Used in / Usada em

_Not used in a project yet / Ainda não usada em projeto._
