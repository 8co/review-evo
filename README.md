# ReviewEvo

Self-improving code reviewer that learns your codebase over time.

ReviewEvo analyzes git history, identifies churn hotspots, learns team conventions, and builds a persistent knowledge base that sharpens every review. It gets smarter the more you use it.

## Install

```
npx clawhub@latest install review-evo
```

## What It Does

1. **Detects your project** — language, framework, build tools
2. **Analyzes git history** — churn hotspots, contributor patterns, complexity signals
3. **Builds a review profile** — conventions, risks, strengths
4. **Delivers targeted findings** — full health report, PR review, or focused file analysis
5. **Stores learnings** — persists findings in `.review-evo/learnings.md` so the next review builds on the last

## Requirements

- `git` (that's it)

No API keys. No dependencies. No external services. The skill uses git and the agent's built-in file tools.

## How It Works

The entire product is a single `SKILL.md` file. Your AI agent reads it and follows the instructions using tools it already has. There is no runtime code to install, compile, or execute.

Learnings persist locally in `.review-evo/learnings.md` inside your project. Each review appends new findings. Over time, the agent recognizes recurring patterns, tracks resolved issues, and focuses on what actually matters in your codebase.

## Security

- Zero dependencies
- Zero network calls
- Zero scripts or binaries
- Pure text instructions only
- Passes OpenClaw security scan and VirusTotal

## License

MIT
