# 🚀 Copilot Starter Template

> **One command. Personalized Copilot ecosystem. Any project.**

This template contains portable agents and prompts that bootstrap a complete GitHub Copilot infrastructure tailored specifically to YOUR project's needs.

## Quick Start

### Option 1: Use This Template
1. Click **"Use this template"** → **"Create a new repository"**
2. Clone and open in VS Code
3. In Copilot Chat, select **copilotBootstrap** from the agent list, then type:
   ```
   Set up Copilot for this project
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

Then reload VS Code and select **copilotBootstrap** from the agent list.

## How It Works

The bootstrap agent **asks about your project first**, then finds suitable resources:

```
👋 Welcome to Copilot Bootstrap!

Tell me about your project:
1. What type? (web app, API, CLI, library, mobile app)
2. What tech? (React, Python, Node.js, .NET, etc.)
3. Main purpose?
4. Focus areas? (accessibility, security, testing)

Or just describe it and I'll figure it out!
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

| Agent | How to Use | Description |
|-------|------------|-------------|
| `copilot-bootstrap.agent.md` | Select **copilotBootstrap** | Primary entry point - asks about project, finds resources |
| `meta-agentic-project-scaffold.agent.md` | Select from list | Extensive awesome-copilot discovery |

### Prompts (`.github/prompts/`)

| Prompt | Description |
|--------|-------------|
| `suggest-awesome-github-copilot-agents.prompt.md` | Find agents relevant to your project |
| `suggest-awesome-github-copilot-collections.prompt.md` | Find collections (bundled resources) |
| `suggest-awesome-github-copilot-instructions.prompt.md` | Find instructions for your tech stack |
| `suggest-awesome-github-copilot-prompts.prompt.md` | Find prompts for your workflows |

## Commands

### Primary Command
Select **copilotBootstrap** from the agent dropdown, then:
```
Set up Copilot for this project
```

### With Context
```
Set up Copilot for this React/TypeScript e-commerce app with focus on accessibility
```

### After Setup - Daily Use
| Agent | Description |
|-------|-------------|
| **orchestrator** | Coordinate complex tasks |

## Example Setup Flow

```
You: [Select copilotBootstrap] Set up Copilot for this project

Bot: 👋 Welcome! Tell me about your project...

You: This is a Python FastAPI backend for a health tracking app. 
     Focus on security and testing.

Bot: 📋 Project Summary:
     - Type: API/Backend
     - Tech: Python, FastAPI
     - Focus: Security, Testing
     
     Ready to find suitable Copilot resources?

You: Yes

Bot: Based on your project, I recommend:
     | Resource | Type | Why Relevant |
     |----------|------|--------------|
     | debug.agent.md | Agent | Essential debugging |
     | python.instructions.md | Instructions | Python standards |
     | secure-code-review.prompt.md | Prompt | Security focus |
     
     Install all, or pick specific ones?

You: Install all

Bot: ✅ Done! Created orchestrator and copilot-instructions.md
```

## Important Notes

- **Agent names use camelCase**: The agent shows as `copilotBootstrap` in the list
- **Reload VS Code** after adding agent files for them to appear
- **Select from dropdown**: Click the agent dropdown in Copilot Chat to see available agents

## Documentation

See [awesome-copilot-quickstart-mj.md](awesome-copilot-quickstart-mj.md) for the complete guide.

## Source

All resources from [github/awesome-copilot](https://github.com/github/awesome-copilot).

## License

MIT
