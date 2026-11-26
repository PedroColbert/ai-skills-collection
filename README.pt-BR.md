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
| [animate](animate/STUDY.md) | Animação | Cria uma animação decidindo na ordem certa (deve animar? → curva → saída) | [emilkowalski/skills](https://github.com/emilkowalski/skills) |
| [choreograph](choreograph/STUDY.md) | Animação | Coordena vários elementos para o grupo se mover como um só | [emilkowalski/skills](https://github.com/emilkowalski/skills) |
| [gsap-scrolltrigger](gsap-scrolltrigger/STUDY.md) | Animação / GSAP | Skill oficial do GSAP: animação na rolagem, seções presas, scrub | [greensock/gsap-skills](https://github.com/greensock/gsap-skills) |
| [gsap-plugins](gsap-plugins/STUDY.md) | Animação / GSAP | Skill oficial do GSAP: SplitText, Flip, Draggable, MorphSVG… (todos grátis) | [greensock/gsap-skills](https://github.com/greensock/gsap-skills) |
| [frontend-design](frontend-design/STUDY.md) | Web design | Direção visual marcante que não parece template | [anthropics/skills](https://github.com/anthropics/skills) |
| [build-awwwards-quality-sites](build-awwwards-quality-sites/STUDY.md) | Web design | Sites de portfólio e landing pages com direção de arte e animação | [MengTo/Skills](https://github.com/MengTo/Skills) |
| [awwwards](awwwards/STUDY.md) | Web design | Sites nível prêmio a partir de um briefing curto, com QA por crítico cego | [juliobsz/skills](https://github.com/juliobsz/skills) |
| [jury](jury/STUDY.md) | Web design | Dá notas a um site como o júri do Awwwards, a partir de screenshots e métricas | [juliobsz/skills](https://github.com/juliobsz/skills) |
| [ui-ux-pro-max](ui-ux-pro-max/STUDY.md) | UI/UX | Banco local pesquisável de estilos, paletas, fontes e regras de UX | [nextlevelbuilder/ui-ux-pro-max-skill](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill) |
| [emil-design-eng](emil-design-eng/STUDY.md) | Acabamento de UI | Detalhes de design engineering que deixam a interface ótima | [emilkowalski/skills](https://github.com/emilkowalski/skills) |
| [better-ui](better-ui/STUDY.md) | Acabamento de UI | Valores exatos para bordas, sombras, ícones e animações | [jakubkrehel/skills](https://github.com/jakubkrehel/skills) |
| [better-colors](better-colors/STUDY.md) | Design system | Paletas em escala, tokens semânticos, contraste medido | [jakubkrehel/skills](https://github.com/jakubkrehel/skills) |
| [better-typography](better-typography/STUDY.md) | Tipografia | Escala tipográfica, espaçamento, recursos da fonte, quebras | [jakubkrehel/skills](https://github.com/jakubkrehel/skills) |
| [better-layout](better-layout/STUDY.md) | Layout | Agrupamento, alinhamento e layouts que aguentam tradução e espelhamento | [jakubkrehel/skills](https://github.com/jakubkrehel/skills) |
| [web-design-guidelines](web-design-guidelines/STUDY.md) | Revisão de UI | Audita o código da interface pelas diretrizes da Vercel | [vercel-labs/agent-skills](https://github.com/vercel-labs/agent-skills) |
| [copywriting](copywriting/STUDY.md) | Conteúdo | Textos de página com afirmações comprováveis e sem cara de IA | [coreyhaines31/marketingskills](https://github.com/coreyhaines31/marketingskills) |
| [animate-expo](animate-expo/STUDY.md) | Animação / React Native | Sequência de animação para Expo: Reanimated, gestos, vibração | [emilkowalski/skills](https://github.com/emilkowalski/skills) |
| [gestures](gestures/STUDY.md) | Animação | Arrastar, deslizar e sheets que seguem o dedo e podem ser interrompidos | [emilkowalski/skills](https://github.com/emilkowalski/skills) |
| [animation-performance](animation-performance/STUDY.md) | Animação / Desempenho | Descobre por que a animação engasga; só propriedades baratas | [emilkowalski/skills](https://github.com/emilkowalski/skills) |
| [find-animation-opportunities](find-animation-opportunities/STUDY.md) | Animação / Auditoria | Só leitura: onde animar ajudaria e onde não | [emilkowalski/skills](https://github.com/emilkowalski/skills) |
| [remove-animations](remove-animations/STUDY.md) | Animação / Limpeza | Remove animações desnecessárias (só subtrai) | [emilkowalski/skills](https://github.com/emilkowalski/skills) |
| [improve-animations](improve-animations/STUDY.md) | Animação / Auditoria | Auditoria de animações + planos prontos para outros agentes | [emilkowalski/skills](https://github.com/emilkowalski/skills) |
| [review-animations](review-animations/STUDY.md) | Animação / Revisão | Revisão rigorosa por 10 padrões (`/review-animations`) | [emilkowalski/skills](https://github.com/emilkowalski/skills) |
| [animation-vocabulary](animation-vocabulary/STUDY.md) | Animação | Glossário: descrição vaga → nome exato do efeito | [emilkowalski/skills](https://github.com/emilkowalski/skills) |
| [apple-design](apple-design/STUDY.md) | Princípios de design | Princípios de interface e movimento da Apple (WWDC), para a web | [emilkowalski/skills](https://github.com/emilkowalski/skills) |
| [mobile-native](mobile-native/STUDY.md) | Web mobile | Faz o site parecer app no celular (100vh, zoom, hover preso…) | [emilkowalski/skills](https://github.com/emilkowalski/skills) |
| [break-ui](break-ui/STUDY.md) | QA | Testa a interface com dados extremos num botão só de desenvolvimento | [emilkowalski/skills](https://github.com/emilkowalski/skills) |
| [prototype](prototype/STUDY.md) | Exploração de design | Várias versões reais com seletor ao vivo (`/prototype`) | [emilkowalski/skills](https://github.com/emilkowalski/skills) |
| [learn-taste](learn-taste/STUDY.md) | Memória de design | Transforma correções de design em regras no DESIGN.md (`/learn-taste`) | [emilkowalski/skills](https://github.com/emilkowalski/skills) |
| [pick-ui-library](pick-ui-library/STUDY.md) | Ferramentas | Biblioteca certa para cada tarefa de frontend (`/pick-ui-library`) | [emilkowalski/skills](https://github.com/emilkowalski/skills) |
| [ask-sonner](ask-sonner/STUDY.md) | Guia de biblioteca | Guia do Sonner, biblioteca de notificações para React | [emilkowalski/skills](https://github.com/emilkowalski/skills) |
| [ask-emil](ask-emil/STUDY.md) | Roteador | Qual skill do Emil (ou sequência) serve para o seu caso (`/ask-emil`) | [emilkowalski/skills](https://github.com/emilkowalski/skills) |
| [write-swift](write-swift/STUDY.md) | Swift | Swift moderno: concorrência do Swift 6, tipos por valor, Swift Testing | [emilkowalski/skills](https://github.com/emilkowalski/skills) |

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
