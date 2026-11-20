# reanimate — Study / Estudo

| | |
|---|---|
| **Source / Origem** | [NiazMorshed2007/reanimate](https://github.com/NiazMorshed2007/reanimate) (MIT, ~1.9k ⭐, commit `3f7a55a`) |
| **Area / Área** | Frontend / Motion / Animation |
| **Added / Adicionada** | 2026-11-19 |
| **Runs code? / Executa código?** | **Yes** — Bun + TypeScript scripts with Playwright (headless Chromium), ffmpeg and pixelmatch. ~250 MB on first setup. |

---

## 🇺🇸 English

**What it does.** Reverse-engineers an animation **frame by frame** from a reference (live URL, screen recording, mp4/webm/gif, Lottie, prototype export), rebuilds it in *your* codebase, then **records the clone and compares it to the reference frame by frame**, iterating until timing, easing, sequence and layout match. The deliverable is code **plus evidence** (numbers + side-by-side sheets), never "looks about right".

**Fidelity levels** (chosen from the request):
| Level | Must match | May differ |
|---|---|---|
| **motion-faithful** (default) | trigger, order, stagger, timing (±80 ms), easing family, movement relative to size, proportions | copy, colours, fonts, images |
| **pixel-faithful** | all of the above + fonts, colours, spacing, assets; mean mismatch ≤ 2 % | nothing |
| **mixed** | cloned parts at one of the above | your additions |

**Workflow (all artefacts in `.reanimate/<name>/`).**
0. **Scope** → `spec.md`: target, destination stack, fidelity.
1. **Setup** → `bash scripts/setup.sh` (installs Playwright, ffmpeg, pixelmatch).
2. **Capture the reference** → `capture.ts` (website: video, frames, `inspect.json` with declared CSS/WAAPI animations, keyframes, fonts, libraries; `track.json` with per-frame position/opacity/transform), `frames.ts` (video/gif), `--gl --clock virtual` for canvas/WebGL/three.js (dumps shaders, uniforms, scene graph). Build filmstrip sheets and **read every one**.
3. **Motion spec** → one row per element per property (start, duration, stagger, from→to, easing). Numbers come from `inspect.json` → `easing.ts` → reading frames.
4. **Build** in the project's existing stack/animation lib.
5. **Verify loop** → capture the clone with the *same* command, run `compare.ts`, `sheet.ts compare`, `easing.ts --compare-track`. Fix the smallest thing, repeat (2–5 rounds). After 5 failing rounds, report honestly instead of lowering thresholds.
6. **Report** → files, trigger, last-round table, sheets, residual deviations with reasons.

**Scripts.**
| Script | Role |
|---|---|
| `capture.ts` | Playwright recorder: triggers load/scroll/hover/leave/move/drag/click/none, crop, tracking, virtual clock, asset & GL dump |
| `frames.ts` | video/gif → numbered PNG frames (ffmpeg) |
| `sheet.ts` | filmstrip & side-by-side compare sheets |
| `compare.ts` | per-frame pixel mismatch report |
| `easing.ts` | fits easing curves, detects overshoot / spring-like motion |
| `gl.ts` | summarises and compares WebGL captures |

**Smart ideas worth learning.**
- *Same capture for reference and clone* — otherwise you measure your setup, not your work.
- *Virtual clock + seed* makes canvas/random animations deterministic and comparable.
- Read real values (`inspect.json`, shader sources) before estimating from pixels.
- Easing lives in the **middle frames**, not first/last.
- Scroll-driven motion is a function of scroll position, not time.

**When to use.** "Make this hero/loader/carousel/hover move like site X", recreating an animation from a gif or video, porting a prototype's motion into React/Vue/etc., matching a WebGL effect.

**When NOT to use.** Simple animations you can just write; when you can't get a recording (login walls → ask for a screen recording).

**⚠️ Caveats.**
- Needs **Bun** (`powershell -c "irm bun.sh/install.ps1 | iex"`), not installed on this machine yet. `setup.sh` is a bash script → run it from Git Bash on Windows.
- `setup.sh` creates `scripts/node_modules` inside the skill (ignored by this repo's `.gitignore`).
- **Ethics/legal:** cloning *motion* is learning; copying another company's brand, logos, images, copy or proprietary shaders is not OK for production. Default to motion-faithful with your own content.
- Safety review (2026-11-19): no outbound calls besides the page being captured; deletions only inside its own output folders; `--pre-js` runs code *you* pass into the captured page.
- Add `.reanimate/` to the project's `.gitignore`.

## 🇧🇷 Português

**O que faz.** Faz engenharia reversa de uma animação **quadro a quadro** a partir de uma referência (site, gravação de tela, mp4/gif, Lottie, protótipo), reconstrói no *seu* código e depois **grava o clone e compara com a referência quadro a quadro**, repetindo até tempo, easing, sequência e layout baterem. Entrega código **com provas** (números e folhas lado a lado).

**Níveis de fidelidade.** *motion-faithful* (padrão: o movimento bate, conteúdo pode ser seu), *pixel-faithful* (idêntico, ≤ 2 % de diferença), *mixed* (clona uma parte e adiciona coisas suas).

**Fluxo.** Escopo → setup → capturar referência → escrever a especificação do movimento → construir → **verificar, corrigir, repetir** (2–5 rodadas) → relatório com números e desvios restantes.

**Ideias espertas para aprender.**
- Capturar referência e clone com o **mesmo** comando.
- **Relógio virtual + seed** deixam animações de canvas/aleatórias determinísticas.
- Ler os valores reais (animações declaradas, shaders) antes de estimar pelos pixels.
- O easing está nos **quadros do meio**.
- Animação de scroll depende da posição do scroll, não do tempo.

**Quando usar.** "Faz esse hero/loader/carrossel/hover se mexer igual ao do site X", recriar animação de um gif/vídeo, portar a animação de um protótipo, efeitos WebGL/three.js.

**Quando NÃO usar.** Animações simples que dá para escrever direto; quando não há como gravar a referência.

**⚠️ Cuidados.**
- Precisa do **Bun** (ainda não instalado nesta máquina). No Windows, rodar `setup.sh` pelo Git Bash.
- Primeira execução baixa ~250 MB (Chromium + ffmpeg).
- **Ética/jurídico:** clonar o *movimento* é aprendizado; copiar marca, logos, imagens, textos ou shaders de outra empresa para produção não é. Preferir motion-faithful com conteúdo próprio.
- Revisão de segurança (2026-11-19): sem chamadas de rede além da página capturada; só apaga arquivos dentro das próprias pastas de saída.

---

## 🔗 Pairs with / Combina com
`mobile-ios-design` / `mobile-android-design` (only the motion principles transfer — reanimate targets web), any frontend/design skill added later.

## 🧪 Used in / Usada em

_Not used in a project yet / Ainda não usada em projeto._
