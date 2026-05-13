# Weekly Report Skill

Skill operacional para criação, manutenção e evolução do Report Semanal Gnatus/Branevo.

Esta skill documenta os padrões oficiais de:

- estrutura visual dos slides 16:9;
- modo apresentação;
- animações canônicas;
- fluxo de dados semanal;
- templates de novas semanas;
- templates de novos slides;
- critérios para Codex, Gemini CLI e Claude Code trabalharem sem quebrar o produto.

## Instalação rápida

### Claude Code

Clone este repositório dentro da pasta de skills do Claude:

```bash
git clone https://github.com/marcotuliobrz/weekly-report-skill.git ~/.claude/skills/weekly-report-skill
```

Depois reinicie o Claude Code.

### Gemini CLI

Clone o repositório em uma pasta de referência do seu projeto:

```bash
git clone https://github.com/marcotuliobrz/weekly-report-skill.git ./skills/weekly-report-skill
```

Use no prompt:

```text
Leia ./skills/weekly-report-skill/SKILL.md antes de alterar o Report Semanal.
Siga também os arquivos em ./skills/weekly-report-skill/references/.
```

### Codex

Clone o repositório dentro do projeto ou use como referência externa:

```bash
git clone https://github.com/marcotuliobrz/weekly-report-skill.git ./skills/weekly-report-skill
```

No prompt do Codex, use:

```text
Antes de modificar o Report Semanal, leia skills/weekly-report-skill/SKILL.md e aplique os padrões definidos nos arquivos references/ e templates/.
```

## Estrutura

```text
weekly-report-skill/
├── SKILL.md
├── README.md
├── install.md
├── prompts/
│   ├── codex.md
│   ├── gemini-cli.md
│   └── claude-code.md
├── references/
│   ├── architecture.md
│   ├── presentation-mode.md
│   ├── data-flow.md
│   ├── animations.md
│   └── slide-catalog.md
└── templates/
    ├── new-week.ts
    └── new-slide.tsx
```

## Uso recomendado

Use esta skill sempre que for pedir para uma IA:

- criar uma nova semana do report;
- adicionar slide recorrente;
- ajustar modo apresentação;
- mexer em `MeetingHero`, `BuTitleSlide`, `BuOpener`, `ReportTemplate` ou slides de BU;
- consumir dados de `/api/semanal/*`;
- padronizar animações e estrutura visual.

## Princípio principal

Não improvisar estrutura visual, animação ou fluxo de dados. O Report Semanal é um artefato executivo e cinematográfico, com padrões fechados.
