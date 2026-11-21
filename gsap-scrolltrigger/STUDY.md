# gsap-scrolltrigger — Study / Estudo

| | |
|---|---|
| **Source / Origem** | [greensock/gsap-skills](https://github.com/greensock/gsap-skills/tree/main/skills/gsap-scrolltrigger) (MIT) |
| **Area / Área** | Motion / GSAP |
| **Added / Adicionada** | 2026-11-15 (portfolio project) · collection 2026-11-21 |
| **Runs code? / Executa código?** | No |

---

## 🇺🇸 English

**What it does.** Official GSAP skill for ScrollTrigger: scroll-linked animations, pinning, scrub, batch, scrollerProxy, horizontal scroll.

**How it works.** One `SKILL.md`: registration, key config, batch, scrollerProxy, scrub, pinning, markers, timelines, `containerAnimation`, refresh & cleanup, best practices, "Do Not" list.

**Core takeaways.**
- Register the plugin; attach ScrollTrigger to timelines, not to each child tween.
- `containerAnimation` for horizontal-scroll sections (the portfolio's pinned projects strip).
- Refresh after images/fonts load; kill triggers on cleanup.
- Use `markers` only in development.
- Recommended default for scroll-driven animation when no library is chosen.

**When to use.** Parallax, pinned sections, scrubbed timelines, scroll reveals.

**When NOT to use.** Simple reveals that CSS scroll-driven animations or IntersectionObserver handle.

## 🇧🇷 Português

**O que faz.** Skill oficial do GSAP para ScrollTrigger: animações ligadas à rolagem, seções presas, scrub, rolagem horizontal.

**Principais lições.**
- Ligar o ScrollTrigger à timeline, não a cada tween.
- `containerAnimation` para rolagem horizontal.
- Atualizar depois de carregar imagens e fontes; limpar ao sair.

**Quando usar.** Parallax, seções presas, animações controladas pela rolagem.

**Quando NÃO usar.** Revelações simples que CSS resolve.

---

## 🔗 Pairs with / Combina com
`gsap-plugins`, `choreograph`, `build-awwwards-quality-sites`

## 🧪 Used in / Usada em

- **2026-11-15 — pedro-colbert-portfolio** (online CV site, Vite + TS + GSAP + React islands): installed as a project skill for the site's design and motion work.
- **2026-11-15 — pedro-colbert-portfolio** (currículo online, Vite + TS + GSAP + ilhas React): instalada como skill do projeto para o design e as animações do site.
