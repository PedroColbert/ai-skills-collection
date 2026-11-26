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

### animate · choreograph
- **EN:** `animate` builds **one** animation by deciding in order (should it animate → purpose → tool → properties → easing → exit → reduced motion). `choreograph` coordinates **several** elements (staggers, hero entrances, view swaps) with no uniform stagger and nothing blocking clicks.
- **PT:** `animate` cria **uma** animação decidindo na ordem certa. `choreograph` coordena **vários** elementos (stagger, entrada do hero, troca de telas).
- **Use when / Usar quando:** adding motion / adicionar animação. **Pairs with / Combina com:** `emil-design-eng`, `gsap-*`.
- 📄 [animate](animate/STUDY.md) · [choreograph](choreograph/STUDY.md)

### gsap-scrolltrigger · gsap-plugins (official GSAP)
- **EN:** Scroll-linked animation, pinning, scrub, horizontal scroll; every GSAP plugin (SplitText, ScrambleText, Flip, Draggable, MorphSVG…) — **all free**, install from public `gsap`.
- **PT:** Animação ligada à rolagem, seções presas, rolagem horizontal; todos os plugins do GSAP — **todos grátis**.
- **Use when / Usar quando:** any GSAP project (e.g. the portfolio) / qualquer projeto com GSAP.
- 📄 [gsap-scrolltrigger](gsap-scrolltrigger/STUDY.md) · [gsap-plugins](gsap-plugins/STUDY.md)

---

## 🎨 Web design & UI

### frontend-design · build-awwwards-quality-sites
- **EN:** Visual direction. `frontend-design` (Anthropic) avoids templated "AI look"; `build-awwwards-quality-sites` art-directs motion-rich portfolio/landing sites (GSAP + one smooth-scroll engine + optional Three.js, honest assets).
- **PT:** Direção visual. `frontend-design` evita a "cara de IA"; `build-awwwards-quality-sites` faz sites de portfólio/landing com direção de arte e animação.
- **Use when / Usar quando:** starting or reshaping a site / começar ou repensar um site. **Avoid / Evitar:** dashboards (awwwards).
- 📄 [frontend-design](frontend-design/STUDY.md) · [build-awwwards-quality-sites](build-awwwards-quality-sites/STUDY.md)

### awwwards · jury
- **EN:** `awwwards` builds award-caliber sites from a short brief (concept → art direction in `DESIGN.md` → GSAP + Lenis build → QA loop with a blind critic until every score ≥ 8). `jury` only scores a site, Awwwards-style, from screenshots, vitals, axe and an SEO audit, with a ranked fix list.
- **PT:** `awwwards` constrói sites nível prêmio a partir de um briefing curto (conceito → direção de arte → GSAP + Lenis → QA com crítico cego até notas ≥ 8). `jury` só avalia um site no estilo do júri do Awwwards, com lista de correções.
- **Use when / Usar quando:** portfolio or landing that must impress; "is it Awwwards-level?" / portfólio ou landing que precisa impressionar; "está no nível Awwwards?". **Avoid / Evitar:** dashboards, app UIs.
- **Requires / Requer:** Node 20+, Playwright + axe-core for QA scripts.
- 📄 [awwwards](awwwards/STUDY.md) · [jury](jury/STUDY.md)

### ui-ux-pro-max
- **EN:** Offline searchable database (styles, palettes, font pairings, UX rules, 22 stacks) + design-system generator (`MASTER.md`). Python 3.
- **PT:** Banco de dados local (estilos, paletas, fontes, regras de UX, 22 stacks) + gerador de design system. Python 3.
- **Use when / Usar quando:** no visual direction yet / ainda sem direção visual.
- 📄 [STUDY.md](ui-ux-pro-max/STUDY.md)

### emil-design-eng · better-ui · better-colors · better-typography · better-layout
- **EN:** Polish layer with exact values: interaction details (Emil), surfaces/icons/motion, colour systems & contrast, typography, layout & i18n.
- **PT:** Camada de acabamento com valores exatos: interações, superfícies, cores e contraste, tipografia, layout.
- **Use when / Usar quando:** final polish or design-system work / acabamento final ou design system.
- 📄 [emil](emil-design-eng/STUDY.md) · [ui](better-ui/STUDY.md) · [colors](better-colors/STUDY.md) · [typography](better-typography/STUDY.md) · [layout](better-layout/STUDY.md)

### web-design-guidelines
- **EN:** Audits UI code against Vercel's Web Interface Guidelines (fetched fresh each review) → `file:line` findings.
- **PT:** Audita o código da interface pelas diretrizes da Vercel (baixadas a cada revisão).
- **Use when / Usar quando:** "review my UI" before shipping / "revise minha UI" antes de publicar. **Needs internet / Precisa de internet.**
- 📄 [STUDY.md](web-design-guidelines/STUDY.md)

---

## 🪄 Emil Kowalski's motion & design toolkit

Full set from [emilkowalski/skills](https://github.com/emilkowalski/skills) (with `animate`, `choreograph`, `emil-design-eng` above). Start with `/ask-emil` if unsure / comece com `/ask-emil` se tiver dúvida.

**Flow / Fluxo:** `/prototype` → build (`animate` · `choreograph` · `gestures` · `animate-expo`) → break it (`break-ui` · `/review-animations`) → `/learn-taste`.

| Situation / Situação | Skill |
|---|---|
| Don't know what it should look like / Não sei como deve ficar | `/prototype` |
| Drag, swipe, sheets / Arrastar, deslizar, sheets | `gestures` · `apple-design` |
| Expo / React Native motion | `animate-expo` |
| Animation is janky / Animação engasgando | `animation-performance` |
| What could animate? / O que dá para animar? | `find-animation-opportunities` |
| Too much motion, app feels slow / Animação demais | `remove-animations` |
| Audit all motion, plans for other agents / Auditar tudo | `improve-animations` |
| Strict motion review before merge / Revisão rigorosa | `/review-animations` |
| Don't know the effect's name / Não sei o nome do efeito | `animation-vocabulary` |
| Site feels wrong on phone / Site estranho no celular | `mobile-native` |
| Edge cases: long names, empty lists / Dados extremos | `break-ui` |
| Which library? / Qual biblioteca? | `/pick-ui-library` · `ask-sonner` |
| Save design decisions for next time / Guardar decisões | `/learn-taste` |
| Swift code | `write-swift` |

Commands in `/slash` form are **manual-only** (`disable-model-invocation`) / Os com `/barra` são **só manuais**.

---

## ✍️ Content / Conteúdo

### copywriting
- **EN:** Page copy after diagnosing the input (blank / real voice / point edit); supportable claims only; no AI tells.
- **PT:** Textos de página depois de diagnosticar o pedido; só afirmações comprováveis; sem cara de IA.
- **Use when / Usar quando:** hero copy, CV text, landing pages / textos de hero, currículo, landing pages.
- 📄 [STUDY.md](copywriting/STUDY.md)

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
