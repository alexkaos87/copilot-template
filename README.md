# GitHub Copilot Common Tools

A reusable collection of GitHub Copilot skills, agents, prompts, and instructions. Use the complete repository as a shared toolbox, or copy the tools you need into another project.

## What's included

### Skills

The skills in [`.agents/skills/`](.agents/skills/) cover:

| Skill | What it helps with |
| --- | --- |
| [code-review](.agents/skills/code-review/) | Review code changes against project standards and requirements. |
| [create-agentsmd](.agents/skills/create-agentsmd/) | Create an `AGENTS.md` file for a repository. |
| [create-readme](.agents/skills/create-readme/) | Write a project README based on the repository contents. |
| [docx](.agents/skills/docx/) | Create, edit, and inspect Word documents. |
| [domain-modeling](.agents/skills/domain-modeling/) | Develop a domain model, glossary, or architecture decision record. |
| [graphify](.agents/skills/graphify/) | Build and query a knowledge graph of code and project materials. |
| [grill-me](.agents/skills/grill-me/) | Sharpen a plan or design through a structured interview. |
| [grill-with-docs](.agents/skills/grill-with-docs/) | Explore a plan or design and capture decisions in documentation. |
| [grilling](.agents/skills/grilling/) | Stress-test a plan, decision, or idea. |
| [improve-codebase-architecture](.agents/skills/improve-codebase-architecture/) | Find and explore opportunities to improve codebase architecture. |
| [pdf](.agents/skills/pdf/) | Create, edit, and inspect PDF documents. |
| [skill-creator](.agents/skills/skill-creator/) | Create, improve, and evaluate agent skills. |
| [xlsx](.agents/skills/xlsx/) | Create, edit, and analyze spreadsheet files. |

### Copilot customizations

- [Agents](.github/agents/): **Instructions Generator** and **Prompt Builder**.
- [Prompt](.github/prompts/create-instructions.prompt.md): generate an instructions file for a project.
- [Instructions](.github/instructions/authoring-language.instructions.md): authoring conventions for skills and Copilot customization files.
- [`skills-lock.json`](skills-lock.json): source and hash metadata for imported skills.

## Use the tools

1. Create a repository from this template if the option is enabled, or clone the repository.
2. To share selected tools with another project, copy the relevant skill folders from `.agents/skills/` and customization files from `.github/`, keeping their directory structure intact.
3. Open the destination repository in VS Code with GitHub Copilot enabled. Use skills by describing the task they cover; select a custom agent or prompt when appropriate.

You can copy one tool at a time; skills may include supporting scripts, assets, or references in addition to their `SKILL.md` file.

> [!IMPORTANT]
> Some bundled skills include their own license files and terms. Check those files before redistributing or adapting a skill; the root `LICENSE` may not cover every bundled component.

## Repository layout

```text
.agents/skills/     Reusable skills and their supporting resources
.github/agents/     Custom Copilot agents
.github/instructions/  Copilot instructions
.github/prompts/    Reusable prompts
skills-lock.json    Imported skill source and hash metadata
```
