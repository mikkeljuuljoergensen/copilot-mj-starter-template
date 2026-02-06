# 🚀 Copilot Starter Template

> **One command. Full Copilot ecosystem. Any project.**

This template contains portable agents and prompts that bootstrap a complete GitHub Copilot infrastructure for any new project.

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
mkdir -p .github/agents .github/prompts

# Download the main bootstrap agent
curl -sL "https://raw.githubusercontent.com/YOUR_USERNAME/copilot-starter-template/main/.github/agents/copilot-bootstrap.agent.md" -o .github/agents/copilot-bootstrap.agent.md
curl -sL "https://raw.githubusercontent.com/YOUR_USERNAME/copilot-starter-template/main/.github/agents/meta-agentic-project-scaffold.agent.md" -o .github/agents/meta-agentic-project-scaffold.agent.md

# Download the suggest-awesome prompts
curl -sL "https://raw.githubusercontent.com/YOUR_USERNAME/copilot-starter-template/main/.github/prompts/suggest-awesome-github-copilot-agents.prompt.md" -o .github/prompts/suggest-awesome-github-copilot-agents.prompt.md
curl -sL "https://raw.githubusercontent.com/YOUR_USERNAME/copilot-starter-template/main/.github/prompts/suggest-awesome-github-copilot-collections.prompt.md" -o .github/prompts/suggest-awesome-github-copilot-collections.prompt.md
curl -sL "https://raw.githubusercontent.com/YOUR_USERNAME/copilot-starter-template/main/.github/prompts/suggest-awesome-github-copilot-instructions.prompt.md" -o .github/prompts/suggest-awesome-github-copilot-instructions.prompt.md
curl -sL "https://raw.githubusercontent.com/YOUR_USERNAME/copilot-starter-template/main/.github/prompts/suggest-awesome-github-copilot-prompts.prompt.md" -o .github/prompts/suggest-awesome-github-copilot-prompts.prompt.md
```

Then run `@copilot-bootstrap Set up Copilot for this project` in VS Code Copilot Chat.

## What's Included

### Agents (`.github/agents/`)

| Agent | Description |
|-------|-------------|
| `copilot-bootstrap.agent.md` | **Primary entry point** - Portable bootstrapper that sets up complete Copilot ecosystem. Can delegate to meta-agentic-project-scaffold when needed. |
| `meta-agentic-project-scaffold.agent.md` | Specialized agent for pulling resources from awesome-copilot and creating workflows |

### Prompts (`.github/prompts/`)

| Prompt | Description |
|--------|-------------|
| `suggest-awesome-github-copilot-agents.prompt.md` | Analyze project and suggest relevant agents from awesome-copilot |
| `suggest-awesome-github-copilot-collections.prompt.md` | Suggest and install collections (bundles of related resources) |
| `suggest-awesome-github-copilot-instructions.prompt.md` | Suggest instruction files based on your tech stack |
| `suggest-awesome-github-copilot-prompts.prompt.md` | Suggest prompt files based on project needs |

## What You Get After Bootstrapping

After running the bootstrap, your project will have:

| Resource Type | Count | Examples |
|---------------|-------|----------|
| **Agents** | 10-15 | orchestrator, debug, mentor, accessibility |
| **Prompts** | 7+ | secure-code-review, generate-unit-tests |
| **Instructions** | 4-8 | a11y, performance, stack-specific |
| **Collections** | 2-3 | frontend, accessibility |

Plus a customized **orchestrator** that coordinates everything!

## Commands

### Primary Command
| Command | Description |
|---------|-------------|
| `@copilot-bootstrap Set up Copilot for this project` | **Start here** - Full setup with orchestrator creation |

### Additional Commands
| Command | Description |
|---------|-------------|
| `@copilot-bootstrap minimal` | Core resources only |
| `@copilot-bootstrap update` | Update existing resources |
| `@meta-agentic-project-scaffold` | Direct access to resource pulling agent |
| `/suggest-awesome-github-copilot-agents` | Find new agents to install |
| `/suggest-awesome-github-copilot-prompts` | Find new prompts to install |
| `/suggest-awesome-github-copilot-instructions` | Find new instructions to install |
| `/suggest-awesome-github-copilot-collections` | Find collections to install |

### After Setup - Daily Use
| Command | Description |
|---------|-------------|
| `@orchestrator` | Coordinate complex tasks |
| `@orchestrator full-review` | Complete code audit |
| `@orchestrator perf-ux` | Performance & UX review |
| `@orchestrator security` | Security audit |

## Workflow Examples

### Initial Project Setup
```
@copilot-bootstrap Set up Copilot for this project
```

### Keep Resources Updated
```
/suggest-awesome-github-copilot-agents
```
Then review the table and ask to install specific agents.

### After Setup - Daily Use
```
@orchestrator Review and improve performance
@orchestrator Security audit this feature
@orchestrator Full code review
```

## Documentation

See [awesome-copilot-quickstart-mj.md](awesome-copilot-quickstart-mj.md) for the complete guide.

## Source

All resources from [github/awesome-copilot](https://github.com/github/awesome-copilot).

## License

MIT
