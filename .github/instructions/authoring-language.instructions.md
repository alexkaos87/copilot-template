---
applyTo: .agents/skills/**/*, .github/**/*
description: "Use when creating, editing, or reviewing a skill file, command file, agent definition file, or rule file."
version: 1.0.0
excludeAgent: false
---

# Authoring Language for Skills, Commands, Agents, and Rules

- Skill files, command files, agent definition files, and rule files MUST be written entirely in English: instructions, headings, examples, table headers, placeholder text, and any other content in the file itself.
- This applies regardless of the language used elsewhere in the conversation, in the codebase, or in the user's request.
- When the user supplies content to be incorporated into one of these files (e.g. pasted requirements, an example, a template, wording to reuse) and that content is not in English, translate it to English before writing it into the file. Do not paste it verbatim in its original language.
- The only exception to this rule is when the user explicitly asks for a file to be written in a language other than English. In that case, the file should be written in the language specified by the user, and the user should be informed that this is a deviation from the standard practice.
