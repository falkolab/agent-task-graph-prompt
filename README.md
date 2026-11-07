# AI Agent Task Graph

An AI-agent prompt for breaking complex tasks into a graph of small, verifiable steps. Supports parallel execution, targeted retries, and resuming work across sessions.

**Language:** English · [Русский](README_ru.md)

## Prompts

- [English prompt](prompt.en.md)
- [Русский промпт](prompt.ru.md)

## How it works

- **Plan:** Split the task into nodes with explicit inputs, outputs, dependencies, and acceptance checks.
- **Execute:** Run independent nodes in parallel and use code for deterministic operations.
- **Validate:** Require observable evidence before accepting results; retry only failed nodes.
- **Resume:** Track decisions, checks, outputs, and remaining work in Markdown files.
- **Control:** Respect permissions, scope, execution limits, and approval gates.

## Usage

1. Open the prompt in your preferred language.
2. Define the six parameters: `{{TASK}}`, `{{OUTPUT}}`, `{{CHECKS}}`, `{{SOURCES}}`, `{{SCOPE}}`, and `{{LIMIT}}`.
3. Give it to an agent with file access, verification tools, and subagent support.
4. Review and approve the proposed task graph before execution.

The workflow uses `graph.md` (task graph), `checks.md` (validation evidence), `progress.md` (handoff state), and `CLAUDE.md` (learned rules). These are output artifacts, not files included in this repository.

## Credits and sources

- [Hoodie (@HoodieFade_) — source post](https://x.com/HoodieFade_/status/2118010863038746652)
- [Andrej Karpathy — autoresearch](https://github.com/karpathy/autoresearch) (methodological inspiration)
- Russian translation and English reconstruction: **Andrey Tkachenko**, [«Автоматизируй это»](https://t.me/aitomateit).

The English prompt is reconstructed from a Spanish-language graphic, not verified against the author's full original English text. This is not a prompt written by Andrej Karpathy.
