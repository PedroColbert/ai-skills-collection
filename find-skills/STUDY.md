# find-skills — Study / Estudo

| | |
|---|---|
| **Source / Origem** | [vercel-labs/skills](https://github.com/vercel-labs/skills/tree/main/skills/find-skills) (MIT, ~40k ⭐) |
| **Area / Área** | Meta / tooling |
| **Added / Adicionada** | 2026-11-14 |
| **Runs code? / Executa código?** | Yes — `npx skills find/add/update` (Node.js required) |

---

## 🇺🇸 English

**What it does.** Turns the agent into a "skill scout": when you ask *"how do I do X?"* or *"is there a skill for X?"*, it searches the open skills ecosystem through the **Skills CLI** (`npx skills`) and the [skills.sh](https://skills.sh/) leaderboard, then recommends and installs skills.

**How it works.**
1. Identifies the domain + task of the request.
2. Checks the skills.sh leaderboard for popular, battle-tested skills.
3. Runs `npx skills find <query>` if needed.
4. **Vets quality** before recommending: install count (prefer 1K+), source reputation (`anthropics`, `vercel-labs`, `microsoft`), GitHub stars.
5. Presents name, purpose, installs, install command and link.
6. Installs on request with `npx skills add <owner/repo@skill> -g -y` (`-g` = global, `-y` = no prompt).

**Key commands.**
```bash
npx skills find react performance      # search
npx skills add vercel-labs/agent-skills@react-best-practices -g -y   # install globally
npx skills update                      # update all
npx skills init my-skill               # scaffold your own
```

**When to use.** Starting a project in a new stack; repetitive tasks that probably have a skill already; looking for new skills to add to this collection.

**When NOT to use.** When an installed skill already covers the task.

**⚠️ Caveats.**
- `-y` skips confirmation — always read a skill's `SKILL.md` and scripts before installing.
- Install count ≠ safety. Low-star, unknown authors deserve a manual review.
- Because this collection lives in `~/.claude/skills` as a git repo, skills installed with `-g` land here and must be committed + documented.

## 🇧🇷 Português

**O que faz.** Transforma o agente num "olheiro de skills": quando você pergunta *"como faço X?"* ou *"tem skill para X?"*, ele busca no ecossistema aberto via **Skills CLI** (`npx skills`) e no ranking do [skills.sh](https://skills.sh/), recomenda e instala skills.

**Como funciona.**
1. Identifica domínio + tarefa do pedido.
2. Consulta o ranking do skills.sh atrás de skills populares e testadas.
3. Roda `npx skills find <busca>` se precisar.
4. **Avalia a qualidade** antes de recomendar: número de instalações (preferir 1K+), reputação da fonte, estrelas no GitHub.
5. Mostra nome, propósito, instalações, comando e link.
6. Instala quando pedido com `npx skills add <dono/repo@skill> -g -y`.

**Quando usar.** Ao começar projeto numa stack nova; tarefas repetitivas que provavelmente já têm skill; para achar skills novas para esta coleção.

**Quando NÃO usar.** Quando uma skill instalada já resolve.

**⚠️ Cuidados.**
- `-y` pula a confirmação — sempre ler o `SKILL.md` e os scripts antes de instalar.
- Muitas instalações ≠ segurança. Autores desconhecidos merecem revisão manual.
- Como esta coleção é um repositório git em `~/.claude/skills`, skills instaladas com `-g` caem aqui e precisam de commit + documentação.

---

## 🧪 Used in / Usada em

_Not used in a project yet / Ainda não usada em projeto._
