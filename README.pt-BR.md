# 🧠 AI Skills Collection

> 🇺🇸 [Read in English](README.md)

Uma coleção viva de **skills para agentes de IA** no [Claude Code](https://claude.com/claude-code), que eu estudo, documento e uso de verdade nos meus projetos.

Cada skill aqui não é só copiada: ela vem com um **arquivo de estudo (`STUDY.md`)** explicando o que faz, quando usar, quando *não* usar, como funciona por dentro e onde eu já apliquei.

## 📚 O que é uma skill?

Uma skill é uma pasta com um arquivo `SKILL.md` que ensina ao agente de IA um fluxo de trabalho ou conhecimento especializado (ex.: "como desenhar interfaces Android nativas com Material 3"). O agente lê a descrição curta da skill e, quando a tarefa combina, carrega as instruções completas sob demanda.

```
nome-da-skill/
├── SKILL.md        ← instruções que o agente lê (nome + descrição no frontmatter)
├── references/     ← documentação extra, carregada só quando necessário
└── STUDY.md        ← minhas anotações sobre a skill (EN + PT)
```

Este repositório fica clonado direto em `~/.claude/skills/`, então toda skill daqui está **ativa** em todas as minhas sessões do Claude Code.

## 🗂️ Skills

| Skill | Área | Para que serve | Origem |
|---|---|---|---|
| [find-skills](find-skills/STUDY.md) | Meta / ferramentas | Descobrir e instalar novas skills do ecossistema aberto | [vercel-labs/skills](https://github.com/vercel-labs/skills) |
| [mobile-android-design](mobile-android-design/STUDY.md) | UI Mobile | Material Design 3 + Jetpack Compose para Android nativo | [wshobson/agents](https://github.com/wshobson/agents) |
| [mobile-ios-design](mobile-ios-design/STUDY.md) | UI Mobile | Apple HIG + SwiftUI para iOS/iPadOS nativo | [wshobson/agents](https://github.com/wshobson/agents) |
| [reanimate](reanimate/STUDY.md) | Frontend / Animação | Clona qualquer animação quadro a quadro e prova que a cópia se mexe igual | [NiazMorshed2007/reanimate](https://github.com/NiazMorshed2007/reanimate) |

## 📦 Estudadas, não instaladas

| Coleção | O que é | Observações |
|---|---|---|
| [ECC — Everything Claude Code](_studies/ecc/STUDY.md) | Kit de "harness" para agentes: 328 skills, 72 agentes, hooks, regras, memória | Analisado quanto a encaixe e riscos; ideias principais e lista de skills para trazer documentadas |

➡️ Detalhes, casos de uso e combinações: **[CATALOG.md](CATALOG.md)**

## 🔁 Como o repositório cresce

1. Encontro uma skill interessante enquanto estudo.
2. Ela é revisada (conteúdo + scripts que executa), instalada e documentada num `STUDY.md`.
3. Sempre que uma skill é usada num projeto real, o projeto entra na seção **"Usada em"** dela.

## ⚖️ Créditos e licenças

Skills de terceiros mantêm seus autores e licenças originais — veja [THIRD_PARTY.md](THIRD_PARTY.md). Minhas anotações e skills próprias estão sob a [Licença MIT](LICENSE).
