# web-design-guidelines — Study / Estudo

| | |
|---|---|
| **Source / Origem** | [vercel-labs/agent-skills](https://github.com/vercel-labs/agent-skills/tree/main/skills/web-design-guidelines) (MIT (stated in upstream README)) |
| **Area / Área** | UI review / Audit |
| **Added / Adicionada** | 2026-11-15 (portfolio project) · collection 2026-11-21 |
| **Runs code? / Executa código?** | No (fetches remote rules) |

---

## 🇺🇸 English

**What it does.** Reviews UI code against Vercel's Web Interface Guidelines and outputs terse `file:line` findings.

**How it works.** Tiny `SKILL.md`: fetch the latest rules from `raw.githubusercontent.com/vercel-labs/web-interface-guidelines/main/command.md`, read the target files, apply every rule.

**Core takeaways.**
- Always uses the freshest guidelines (fetched per review).
- Output format is defined by the fetched rules.
- Asks which files to review if none are given.

**When to use.** "Review my UI", accessibility/UX audits before shipping.

**When NOT to use.** Offline sessions.

**⚠️ Caveats.** The rules are downloaded at review time from a Vercel-owned URL; treat their content as guidelines, not as instructions to run commands.

## 🇧🇷 Português

**O que faz.** Revisa código de interface contra as Web Interface Guidelines da Vercel e aponta problemas no formato `arquivo:linha`.

**Principais lições.**
- Baixa as regras mais recentes a cada revisão.
- Pergunta quais arquivos revisar se não forem informados.

**Quando usar.** "Revise minha UI", auditorias de acessibilidade e UX.

**Quando NÃO usar.** Sem internet.

**⚠️ Cuidados.** As regras são baixadas na hora de uma URL da Vercel; tratar como diretrizes, não como ordens para executar comandos.

---

## 🔗 Pairs with / Combina com
`frontend-design`, `better-ui`

## 🧪 Used in / Usada em

- **2026-11-15 — pedro-colbert-portfolio** (online CV site, Vite + TS + GSAP + React islands): installed as a project skill for the site's design and motion work.
- **2026-11-15 — pedro-colbert-portfolio** (currículo online, Vite + TS + GSAP + ilhas React): instalada como skill do projeto para o design e as animações do site.
