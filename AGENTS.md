# AGENTS.MD — ReviewEvo

## Project

- **Purpose:** Self-improving code review skill for AI agents
- **Stack:** Pure markdown (SKILL.md) — no runtime code
- **License:** MIT

## How It Works

`skills/SKILL.md` is the entire product. An AI agent reads it and follows the instructions using git and its built-in tools. No compilation, no dependencies, no build step.

## Rules for Agents

1. **Read before writing.** Understand the SKILL.md before proposing changes.
2. **Keep SKILL.md under 4,000 tokens.** This is a hard constraint for prompt budget.
3. **No code, no scripts, no binaries.** The skill is text-only.
4. **No network commands.** Only `git` and local file reads/writes.
5. **No obfuscation.** Every instruction must be human-readable.
6. **Test by running the skill.** Open a real git repo and follow the SKILL.md step by step.
