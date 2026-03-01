# Life OS

A personal filesystem that works as your life operating system — designed to be read, queried, and operated on by an AI agent.

## What This Is

Life OS is a structured set of markdown files that give an AI agent (Goose, Claude, or any LLM with filesystem access via MCP) persistent context about your life — who you are, what you're working on, what you're learning, and what's happened. The AI reads these files at the start of every session and operates on your life with the same coherence an operating system operates on system state.

## Quick Start

1. Clone this repo to your machine
2. Open the folder with your AI agent (Goose, Claude Code, etc.)
3. Tell the agent: **"Read SETUP.md and help me configure my Life OS"**
4. Answer the agent's questions — setup takes ~5 minutes
5. Start using it

## How It Works

```
You ←→ AI Agent ←→ Life OS Filesystem (via MCP)
```

The AI agent connects to your filesystem through MCP (Model Context Protocol). It can read any file for context and write updates when you make decisions, complete tasks, or capture new information.

## Structure

| Folder | Purpose | Changes How Often |
|--------|---------|-------------------|
| `me/` | Who you are, how the system works, what tools are available | Weekly or less |
| `learn/` | What you're actively studying or researching | As needed |
| `do/` | Active projects and life area indexes | Daily |
| `log/` | Journal entries, decision records | Daily (append-only) |

## Key Principle

**The filesystem is the single source of truth.** The AI has no memory between sessions. Everything it knows about you comes from these files. Keep them current, and the AI stays current.

## Creating New Things

- **New project:** Copy `do/_project-template/` to `do/your-project-name/`
- **New learning topic:** Copy `learn/_template.md` to `learn/your-topic.md`
- **New skill:** Copy `me/skills/_template.md` to `me/skills/your-skill.md`
- **New journal entry:** Copy `log/journal/_template.md` to `log/journal/YYYY-MM-DD.md`

Or just ask your AI agent to create them — it knows the templates.
