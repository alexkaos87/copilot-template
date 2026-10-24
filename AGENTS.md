# AGENTS.md

## Project Overview

This repository is a collection of reusable GitHub Copilot skills and customizations. It is not an application: there is no root package manifest, build system, or test suite.

- `.agents/skills/` contains skills and their supporting resources, such as scripts, assets, references, and licenses.
- `.github/agents/` contains custom Copilot agents.
- `.github/prompts/` contains reusable prompts and instruction files.
- `.github/instructions/` contains authoring guidance.
- `skills-lock.json` records source and hash metadata for imported skills.

For the human-oriented overview and skill descriptions, see [README.md](README.md).

## Setup and Development

This is a documentation and reusable-tool repository. Clone it and open it in the editor of your choice; no dependency installation, environment setup, database, or development server is required for repository-level work. There is no root package manifest or standard build/watch command.

Before making a change:

1. Read the relevant skill's `SKILL.md` before editing that skill or its supporting resources.
2. Read nearby examples and preserve the existing file format and folder structure.
3. For skill and Copilot customization content, follow [.github/instructions/authoring-language.instructions.md](.github/instructions/authoring-language.instructions.md). Write these files in English unless the user explicitly requests another language.
4. Check bundled license or terms before adapting or redistributing content. The root `LICENSE` may not cover every bundled component.

When adding, removing, or renaming a skill or customization, update the README inventory and descriptions. Keep `skills-lock.json` consistent when changing imported-skill source or hash metadata; do not change it for unrelated edits.

## Available skills

The current skill directories under `.agents/skills/` are:

- `code-review`
- `create-agentsmd`
- `create-readme`
- `docx`
- `domain-modeling`
- `graphify`
- `grill-me`
- `grill-with-docs`
- `grilling`
- `improve-codebase-architecture`
- `pdf`
- `skill-creator`
- `xlsx`

Consult each skill’s `SKILL.md` for its scope, workflow, and any required tools or supporting files.

## Copilot Customizations

- Agents: [Instructions Generator](.github/agents/instructions-generator.agent.md) and [Prompt Builder](.github/agents/prompt-builder.agent.md).
- Prompt: [Create instructions](.github/prompts/create-instructions.prompt.md).
- Reusable instruction file: [Practical Design Principles](.github/instructions/solid-kiss-dry.instructions.md).
- Authoring rules: [.github/instructions/authoring-language.instructions.md](.github/instructions/authoring-language.instructions.md).

When adding a customization, use the appropriate existing directory and follow its established file format and conventions. Keep the README's customization inventory current.

## Style and Validation

- There are no repository-wide build, lint, or test commands configured at the root. Do not install project dependencies or invent commands that are not defined by the relevant skill.
- For Markdown or customization changes, review the rendered content, verify relative links and referenced paths, and run `git diff --check` to detect whitespace errors.
- For changes to a skill, follow the validation instructions in that skill's `SKILL.md`; validate any affected scripts with the checks documented by that skill.
- Keep changes focused and preserve existing terminology, conventions, and supporting files. Do not alter unrelated or bundled third-party content.

## Build and Deployment

There is no root application build or deployment process. Individual skills may include scripts or their own validation requirements; consult the skill documentation before running or changing them. No repository-wide CI workflow is configured.

## Pull Requests

No repository-specific title or commit-message format is defined. Before proposing a change, review the final diff and run `git diff --check`. Include a concise description of the user-facing or agent-facing change and report any skill-specific validation performed.

## Security and Scope

Do not add secrets or credentials. Respect the license and terms of each bundled component. Avoid changing bundled third-party skill content or license files unless the change is necessary and authorized.
