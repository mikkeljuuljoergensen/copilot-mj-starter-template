# 🚀 Copilot Starter Template

> **One command. Full Copilot ecosystem. Any project.**

This template contains a single portable agent that bootstraps a complete GitHub Copilot infrastructure for any new project.

## Quick Start

### Option 1: Use This Template
1. Click **"Use this template"** → **"Create a new repository"**
2. Clone and open in VS Code
3. In Copilot Chat, run:
   ```
   @copilot-bootstrap Set up Copilot for this project
   ```

### Option 2: Add to Existing Project
```bash
mkdir -p .github/agents && curl -sL "https://raw.githubusercontent.com/YOUR_USERNAME/copilot-starter-template/main/.github/agents/copilot-bootstrap.agent.md" -o .github/agents/copilot-bootstrap.agent.md
```

Then run `@copilot-bootstrap` in VS Code Copilot Chat.

## What You Get

After bootstrapping, your project will have:

| Resource Type | Count | Examples |
|---------------|-------|----------|
| **Agents** | 10-15 | orchestrator, debug, mentor, accessibility |
| **Prompts** | 7+ | secure-code-review, generate-unit-tests |
| **Instructions** | 4-8 | a11y, performance, stack-specific |
| **Collections** | 2-3 | frontend, accessibility |

Plus a customized **orchestrator** that coordinates everything!

## Commands

| Command | Description |
|---------|-------------|
| `@copilot-bootstrap` | Full setup |
| `@copilot-bootstrap minimal` | Core resources only |
| `@orchestrator` | Coordinate complex tasks |
| `@orchestrator full-review` | Complete audit |

## Documentation

See [awesome-copilot-quickstart-mj.md](awesome-copilot-quickstart-mj.md) for the complete guide.

## Source

All resources from [github/awesome-copilot](https://github.com/github/awesome-copilot).

## License

MIT
