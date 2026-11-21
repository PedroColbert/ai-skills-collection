# ECC (Everything Claude Code) — Study / Estudo

| | |
|---|---|
| **Source / Origem** | [affaan-m/ECC](https://github.com/affaan-m/ECC) (MIT, ~308k ⭐, ~45k forks, v2.2) |
| **Type / Tipo** | **Not a single skill — a full "agent harness" toolkit** / **Não é uma skill — é um kit completo de "harness" para agentes** |
| **Area / Área** | Workflow, quality, security, memory, multi-agent |
| **Studied / Estudado** | 2026-11-20 |
| **Installed? / Instalado?** | **No** — study only (decision on 2026-11-20) / **Não** — só estudo |
| **Runs code? / Executa código?** | Yes, if installed: 28 hooks on every session event, Node.js scripts, optional npm CLI (`ecc-universal`) and MCP server |

---

## 🇺🇸 English

### What it is
A whole engineering system for coding agents (Claude Code first, plus Codex, Cursor, OpenCode, Gemini, Zed, Copilot…). Its motto: *"Optimize the context window. Persist everything else."* It pushes the agent through a disciplined loop:

```text
plan -> test -> implement -> review -> verify -> remember -> improve
```

### What's inside
| Component | Count | Role | Context cost |
|---|---:|---|---|
| **Skills** | 328 | Reusable workflows (TDD, security, research, frontend, data, ML, ops, niche domains) | Loaded only when needed |
| **Agents** | 72 | Subagents with their own context & tools: `planner`, `architect`, `tdd-guide`, `code-reviewer`, `security-reviewer`, `build-error-resolver`, `e2e-runner`, `refactor-cleaner`… | Isolated |
| **Commands** | 99 | Slash entry points (`/ecc:plan`, `/build-fix`, `/refactor-clean`, `/save-session`…), being migrated to skills | — |
| **Rules** | per language | Always-loaded standards (`common/`, `typescript/`, `python/`…) | **Always loaded** → install selectively |
| **Hooks** | 28 | Scripts on tool events: pre-commit lint, Prettier, `tsc --noEmit` after edits, console.log audits, session save/restore, pattern extraction, cost tracking | Outside the model, but they act on everything |
| **Memory Vault** | — | Portable Markdown memory shared between harnesses (`.ecc/memory/`) | On demand |
| **AgentShield** | — | Scans prompts, hooks, MCP config and secrets as an attack surface | — |

### Key ideas worth learning (even without installing)
1. **Separate the jobs:** skills (on demand) vs agents (isolated context) vs rules (always on) vs hooks (deterministic, outside the model). Each has a different context cost.
2. **Fresh-context review:** the same context that wrote the code shouldn't review it; delegate review to a clean subagent.
3. **Evidence-based TDD:** capture the failing test (RED) *before* implementing, then GREEN, then review, then verify build/lint/types/tests.
4. **Hooks enforce what prompts forget:** "please run tsc" is a suggestion; a PostToolUse hook is a guarantee.
5. **Continuous learning:** distil sessions into "instincts" with confidence scores instead of saving giant transcripts.
6. **Treat agent config as attack surface** (prompt injection via hooks/MCP/skills) → scan it.
7. **Research first** (`search-first`): look for an existing package/skill/MCP before writing custom code.

### How to install (if one day we want it)
- **Full plugin:** `/plugin marketplace add https://github.com/affaan-m/ECC` → `/plugin install ecc@ecc`.
- **Low-context, no hooks:** `npx ecc-universal@2.2.3 install --profile minimal --target claude`.
- **Only specific skills:** `./install.sh --target claude --skills tdd-workflow,security-review`, or copy `skills/<name>/` manually.
- Uninstall: `node scripts/ecc.js` (`list-installed`, `doctor`, `repair`) — see README "Reset / Uninstall".

### ⚠️ Why we did NOT install the whole thing
- **Breaks the Windows dev flow:** the *Dev server blocker* hook **blocks `npm run dev` outside tmux** (exit 2). tmux doesn't exist on Windows → the portfolio's `npm --prefix site run dev` would be blocked.
- **Changes every session:** hooks auto-run Prettier (rewrites files), `tsc`, lint on commit, inject context at SessionStart, request extra turns at Stop. Hard to know what is the agent and what is ECC.
- **Overlaps our setup:** its own memory, session summaries and learning system would compete with this collection and the global `CLAUDE.md`.
- **Its manual installer writes into `~/.claude/skills/`** = this public repo → hundreds of folders would pollute the portfolio.
- 328 skills is a catalog, not a toolbox: many are niche (healthcare, DeFi, homelab, logistics…).

### 🎯 Skills worth cherry-picking later (fit Pedro's stack: Vite + TS + React 19 + GSAP)
| Skill | Why |
|---|---|
| `vite-patterns` | config, plugins, build optimisation — portfolio uses Vite 8 |
| `typescript-patterns` | strict types, narrowing, generics — both projects are TS |
| `react-patterns` / `react-performance` | React 19 islands in the portfolio; 70+ perf rules from Vercel |
| `make-interfaces-feel-better` | spacing, typography, hit areas, interaction polish |
| `frontend-a11y` | keyboard, focus, ARIA — custom cursors & menus need it |
| `seo` | structured data, Core Web Vitals — a CV site must be findable |
| `verification-loop` | build + types + lint + tests + diff review → PASS/FAIL report |
| `tdd-workflow` / `e2e-testing` | for InfinityVelha's game logic (`game-core`, `ranking`) |
| `search-first` | research before coding |

⚠️ `motion-*` skills target **motion/react**, not GSAP — less useful for the portfolio. `react-performance` is adapted from `vercel-labs/agent-skills`, which could also be taken from the original.

### When to reach for ECC
Large or team projects that need enforced process (TDD, reviews, security gates); comparing workflows; learning how to design hooks, agents and rules.

## 🇧🇷 Português

### O que é
Um sistema completo de engenharia para agentes de código (principalmente Claude Code, mas também Codex, Cursor, OpenCode etc.). O lema: *"Otimize a janela de contexto. Persista todo o resto."* Ele força o agente a seguir um ciclo: **planejar → testar → implementar → revisar → verificar → lembrar → melhorar**.

### O que tem dentro
- **328 skills** (carregadas só quando precisa).
- **72 agentes** especializados (planejador, arquiteto, revisor de código, revisor de segurança, corretor de build…), cada um com contexto próprio.
- **99 comandos** (`/ecc:plan`, `/build-fix`…).
- **Regras** sempre carregadas por linguagem (instalar com moderação, pois ocupam contexto o tempo todo).
- **28 hooks**: scripts automáticos em cada evento (formatar com Prettier, rodar `tsc`, checar antes do commit, salvar a sessão, extrair padrões…).
- **Memory Vault** (memória portátil entre ferramentas) e **AgentShield** (varredura de segurança da própria configuração do agente).

### Ideias que vale aprender (mesmo sem instalar)
1. **Separar funções:** skill (sob demanda), agente (contexto isolado), regra (sempre ligada), hook (garantia fora do modelo).
2. **Revisão com contexto limpo:** quem escreveu o código não deve revisá-lo.
3. **TDD com provas:** registrar o teste falhando **antes** de implementar.
4. **Hooks garantem o que o prompt esquece.**
5. **Aprendizado contínuo:** transformar sessões em "instintos" com nível de confiança, em vez de guardar conversas gigantes.
6. **Configuração do agente é superfície de ataque** (injeção de prompt via hooks, MCP, skills).
7. **Pesquisar antes de codar:** procurar pacote/skill pronta antes de escrever do zero.

### ⚠️ Por que NÃO instalamos tudo
- **Quebraria o seu fluxo no Windows:** um hook **bloqueia `npm run dev` fora do tmux**, e tmux não existe no Windows. O `npm run dev` do portfólio pararia de funcionar.
- **Muda todas as sessões:** formata arquivos sozinho, roda verificações, injeta contexto e pede turnos extras.
- **Conflita com o que já temos:** memória e aprendizado próprios competiriam com esta coleção e com o `CLAUDE.md` global.
- **O instalador manual escreve em `~/.claude/skills/`**, que é este repositório público: centenas de pastas poluiriam o portfólio.
- Muitas das 328 skills são de nichos que não usamos (saúde, DeFi, homelab, logística…).

### 🎯 Skills que vale trazer depois (servem para a sua stack: Vite + TS + React 19 + GSAP)
`vite-patterns`, `typescript-patterns`, `react-patterns`, `react-performance`, `make-interfaces-feel-better`, `frontend-a11y`, `seo`, `verification-loop`, `tdd-workflow`/`e2e-testing` (para a lógica do InfinityVelha) e `search-first`. As `motion-*` usam **motion/react**, não GSAP, então ajudam menos no portfólio.

### Quando usar o ECC
Projetos grandes ou em equipe que precisam de processo obrigatório (TDD, revisões, portões de segurança), ou para aprender a desenhar hooks, agentes e regras.

---

## 🔗 Pairs with / Combina com
`find-skills` (finding individual ECC skills), `reanimate` (ECC's `verification-loop` uses the same "prove it with evidence" philosophy).

## 🧪 Used in / Usada em

_Studied only, not installed / Só estudado, não instalado._
