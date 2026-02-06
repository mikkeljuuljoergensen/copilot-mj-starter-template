# 🚀 Copilot Starter Template

> **One command. Personalized Copilot ecosystem. Any project.**

This template contains portable agents and prompts that bootstrap a complete GitHub Copilot infrastructure tailored specifically to YOUR project's needs.

## Quick Start

### Option 1: Use This Template
1. Click **"Use this template"** → **"Create a new repository"**
2. Clone and open in VS Code
3. In Copilot Chat, run:
   ```
   @copilot-bootstrap Set up Copilot for this project
   ```
4. **Answer the questions** about your project
5. Review and approve the recommended resources

### Option 2: Add to Existing Project
```bash
mkdir -p .github/agents .github/prompts

# Download the bootstrap agents
curl -sL "https://raw.githubusercontent.com/YOUR_USERNAME/copilot-starter-template/main/.github/agents/copilot-bootstrap.agent.md" -o .github/agents/copilot-bootstrap.agent.md
curl -sL "https://raw.githubusercontent.com/YOUR_USERNAME/copilot-starter-template/main/.github/agents/meta-agentic-project-scaffold.agent.md" -o .github/agents/meta-agentic-project-scaffold.agent.md

# Download the suggest-awesome prompts
curl -sL "https://raw.githubusercontent.com/YOUR_USERNAME/copilot-starter-template/main/.github/prompts/suggest-awesome-github-copilot-agents.prompt.md" -o .github/prompts/suggest-awesome-github-copilot-agents.prompt.md
curl -sL "https://raw.githubusercontent.com/YOUR_USERNAME/copilot-starter-template/main/.github/prompts/suggest-awesome-github-copilot-collections.prompt.md" -o .github/prompts/suggest-awesome-github-copilot-collections.prompt.md
curl -sL "https://raw.githubusercontent.com/YOUR_USERNAME/copilot-starter-template/main/.github/prompts/suggest-awesome-github-copilot-instructions.prompt.md" -o .github/prompts/suggest-awesome-github-copilot-instructions.prompt.md
curl -sL "https://raw.githubusercontent.com/YOUR_USERNAME/copilot-starter-template/main/.github/prompts/suggest-awesome-github-copilot-prompts.prompt.md" -o .github/prompts/suggest-awesome-github-copilot-prompts.prompt.md
```

Then run `@copilot-bootstrap Set up Copilot for this project` in VS Code Copilot Chat.

## How It Works

The bootstrap agent **asks about your project first**, then finds suitable resources:

```
👋 Welcome to Copilot Bootstrap!

Please tell me about your project:
1. What is this project? (e.g., web app, API, CLI tool)
2. What technologies are you using? (e.g., React, Python, Node.js)
3. What's the main purpose?
4. Any special focus areas? (e.g., accessibility, security)
```

Based on your answers, it will:
1. 🔍 Search awesome-copilot for relevant resources
2. 📋 Present recommendations with rationale
3. ✅ Ask for your approval
4. 📥 Download approved resources
5. 🎯 Create a customized orchestrator

**Every project gets its own tailored setup!**

## What's Included

### Agents (`.github/agents/`)

| Agent | Description |
|-------|-------------|
| `copilot-bootstrap.agent.md` | **Primary entry point** - Asks about your project, finds suitable resources |
| `meta-agentic-project-scaffold.agent.md` | Specialized agent for extensive awesome-copilot discovery |

### Prompts (`.github/prompts/`)

| Prompt | Description |
|--------|-------------|
| `suggest-awesome-github-copilot-agents.prompt.md` | Find agents relevant to your project |
| `suggest-awesome-github-copilot-collections.prompt.md` | Find collections (bundled resources) |
| `suggest-awesome-github-copilot-instructions.prompt.md` | Find instructions for your tech stack |
| `suggest-awesome-github-copilot-prompts.prompt.md` | Find prompts for your workflows |

## Commands

### Primary Command
```
@copilot-bootstrap Set up Copilot for this project
```
Asks about your project, then recommends and installs suitable resources.

### With Context
```
@copilot-bootstrap Set up Copilot for this React/TypeScript e-commerce app with focus on accessibility
```
Provides context upfront, may ask follow-up questions.

### Additional Commands
| Command | Description |
|---------|-------------|
| `@copilot-bootstrap minimal` | Core resources only |
| `@copilot-bootstrap update` | Update existing resources |
| `/suggest-awesome-github-copilot-agents` | Find new agents |
| `/suggest-awesome-github-copilot-prompts` | Find new prompts |
| `/suggest-awesome-github-copilot-instructions` | Find new instructions |
| `/suggest-awesome-github-copilot-collections` | Find collections |

### After Setup - Daily Use
| Command | Description |
|---------|-------------|
| `@orchestrator` | Coordinate complex tasks |
| `@orchestrator full-review` | Complete code audit |

## Example Setup Flow

```
You: @copilot-bootstrap Set up Copilot for this project

Bot: 👋 Welcome! Please tell me about your project...

You: This is a Python FastAPI backend for a health tracking app. 
     Focus on security and testing.

Bot: 📋 Here's what I understand:
     - Type: API/Backend
     - Tech: Python, FastAPI
     - Focus: Security, Testing
     
     Based on this, I recommend:
     - debug.agent.md (debugging)
     - python.instructions.md (Python standards)
     - secure-code-review.prompt.md (security)
     - generate-unit-tests.prompt.md (testing)
     ...
     
     Would you like me to install all of these?

You: Yes, install them all

Bot: ✅ Done! Created orchestrator and copilot-instructions.md
```

## Documentation

See [awesome-copilot-quickstart-mj.md](awesome-copilot-quickstart-mj.md) for the complete guide.

## Source

All resources from [github/awesome-copilot](https://github.com/github/awesome-copilot).

## License

MIT
