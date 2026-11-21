# 📖 Catalog / Catálogo

Quick decision guide: which skill fits which situation.
Guia rápido de decisão: qual skill usar em cada situação.

---

## 🛠️ Meta / Tooling

### find-skills
- **EN:** Searches the open skills ecosystem (`npx skills`, skills.sh) and recommends vetted skills.
- **PT:** Busca no ecossistema aberto de skills (`npx skills`, skills.sh) e recomenda skills confiáveis.
- **Use when / Usar quando:** "is there a skill for X?", starting a project in an unfamiliar stack / começando projeto numa stack nova.
- **Avoid / Evitar:** when a skill for it is already installed here / quando já existe skill instalada aqui.
- **Pairs with / Combina com:** any — it's how new skills enter this collection / qualquer uma, é a porta de entrada da coleção.
- 📄 [STUDY.md](find-skills/STUDY.md)

---

## 🎬 Frontend / Motion

### reanimate
- **EN:** Clones an animation from a URL, video, gif or Lottie frame by frame into your codebase, then proves it matches with frame-by-frame comparisons (Playwright + ffmpeg). Handles CSS, JS, canvas, WebGL, three.js.
- **PT:** Clona uma animação de um site, vídeo, gif ou Lottie quadro a quadro para o seu código e prova que bate com comparações quadro a quadro (Playwright + ffmpeg). Funciona com CSS, JS, canvas, WebGL, three.js.
- **Use when / Usar quando:** "make it move like site X", recreate a hero/loader/carousel/hover/scroll effect, port a prototype's motion / "faz igual ao site X", recriar hero/loader/carrossel/hover/scroll.
- **Avoid / Evitar:** trivial animations; copying other brands' assets for production / animações triviais; copiar assets de outras marcas para produção.
- **Requires / Requer:** Bun, ~250 MB first setup.
- **Pairs with / Combina com:** any web frontend skill / qualquer skill de frontend web.
- 📄 [STUDY.md](reanimate/STUDY.md)

---

## 📱 Mobile UI

### mobile-android-design
- **EN:** Material Design 3, Jetpack Compose, dynamic color, adaptive layouts (WindowSizeClass), Navigation Compose.
- **PT:** Material Design 3, Jetpack Compose, cores dinâmicas, layouts adaptativos (WindowSizeClass), Navigation Compose.
- **Use when / Usar quando:** native Android app in Kotlin/Compose / app Android nativo em Kotlin/Compose.
- **Avoid / Evitar:** Flutter, React Native or web apps (only the design principles transfer) / Flutter, React Native ou web (só os princípios de design se aplicam).
- **Pairs with / Combina com:** `mobile-ios-design` (same app on both platforms / mesmo app nas duas plataformas).
- 📄 [STUDY.md](mobile-android-design/STUDY.md)

### mobile-ios-design
- **EN:** Apple Human Interface Guidelines, SwiftUI layouts, NavigationStack/TabView, SF Symbols, Dynamic Type, materials.
- **PT:** Human Interface Guidelines da Apple, layouts SwiftUI, NavigationStack/TabView, SF Symbols, Dynamic Type, materiais.
- **Use when / Usar quando:** native iOS/iPadOS app in SwiftUI / app iOS/iPadOS nativo em SwiftUI.
- **Avoid / Evitar:** UIKit-only legacy code, cross-platform frameworks / código legado só UIKit, frameworks multiplataforma.
- **Pairs with / Combina com:** `mobile-android-design`.
- 📄 [STUDY.md](mobile-ios-design/STUDY.md)

---

## 📦 Studied collections (not installed) / Coleções estudadas (não instaladas)

### ECC — Everything Claude Code
- **EN:** Full agent-harness toolkit: 328 skills, 72 agents, 99 commands, rules, 28 hooks, memory vault, security scanner. Enforces plan → test → implement → review → verify.
- **PT:** Kit completo de "harness": 328 skills, 72 agentes, 99 comandos, regras, 28 hooks, memória e scanner de segurança. Força planejar → testar → implementar → revisar → verificar.
- **Status:** studied only. Full install blocks `npm run dev` on Windows (tmux hook) and changes every session / só estudado; a instalação completa bloqueia `npm run dev` no Windows e muda todas as sessões.
- **Cherry-pick candidates / Candidatas a trazer:** `vite-patterns`, `typescript-patterns`, `react-patterns`, `react-performance`, `make-interfaces-feel-better`, `frontend-a11y`, `seo`, `verification-loop`, `tdd-workflow`, `search-first`.
- 📄 [STUDY.md](_studies/ecc/STUDY.md)

---

## 🔭 Wishlist / Para estudar

Related skills from the same sources worth evaluating / Skills relacionadas das mesmas fontes que vale avaliar:
- `wshobson/agents` → `react-native-design`, `responsive-design`, `accessibility-compliance`, `design-system-patterns`
