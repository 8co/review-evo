# Claude Code — ReviewEvo

ReviewEvo is a self-improving code review skill for AI agents. It analyzes git history, learns project conventions, identifies risk hotspots, and builds a persistent knowledge base that improves over time.

## How It Works

The entire product is `skills/SKILL.md`. There is no runtime code. The skill instructs the agent to use git and its built-in file tools to perform analysis. Learnings persist in `.review-evo/learnings.md` inside the target project.

## Contributing

### Rules
1. Read before writing.
2. The SKILL.md must stay under 4,000 tokens. If it grows past that, trim.
3. No scripts, no binaries, no npm dependencies. The skill must remain pure text.
4. No network calls. The skill uses only `git` and local file operations.
5. No obfuscated content. Everything must be human-readable.
6. Keep it simple. One file does all the work.

### Security Constraints
This skill is published to ClawHub and scanned by OpenClaw and VirusTotal. To stay clean:
- No `curl`, `wget`, or any network-fetching commands
- No `eval`, `exec`, or dynamic code execution
- No base64 encoding/decoding
- No environment variable reading beyond what git needs
- No file operations outside the target project directory
- No process spawning beyond standard git commands
