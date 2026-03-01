# Life OS — Setup Guide

**This file is for the AI agent.** When a user says "help me set up my Life OS" or "read SETUP.md", follow this guide step by step.

## Setup Protocol

You are helping a human configure their Life OS — a personal filesystem you will use as context in every future session. Your job is to ask them questions, then write their answers into the correct files. Be direct. Don't over-explain. Keep it to 5 minutes.

### Step 1: Identity — `me/context.md`

Ask the user these questions one at a time. Write their answers into `me/context.md`.

1. "Give me a one-line description of who you are and what you do."
2. "What are your top 3 priorities right now — the things that should get your time and attention above all else?"
3. "What's one constraint or reality I should always keep in mind when helping you?" (e.g., limited time, specific health condition, budget constraint, timezone)
4. "How do you prefer to communicate? (e.g., blunt and direct, gentle, detailed explanations, minimal)"

### Step 2: Projects — `do/`

Ask: "What are the 2-3 most important things you're actively working on right now? For each, tell me: the name, what life area it falls under (work/health/family/finances/self), and a one-sentence description of what done looks like."

For each project:
- Create a folder `do/[project-name]/`
- Create `README.md` inside it using the template from `do/_project-template/README.md`
- Fill in the details they gave
- Update the relevant `do/areas/[area].md` index file

### Step 3: Learning — `learn/`

Ask: "Is there anything you're actively learning or researching right now? If so, what?"

If yes:
- Create a file in `learn/` for each topic
- Add it to `learn/index.md`

If no, skip. They can add later.

### Step 4: Tools — `me/tools.md`

Ask: "Which AI tools and services do you have connected or want to connect? Common ones: calendar, email, file storage, task manager, code repos, notes app."

Update `me/tools.md` with their answers.

### Step 5: First Log Entry — `log/`

Create today's journal entry in `log/journal/YYYY-MM-DD.md` with:
```
# YYYY-MM-DD

## Setup Day
- Configured Life OS
- Active projects: [list them]
- Current priorities: [list them]
```

Add a first entry to `log/decisions.md`:
```
## YYYY-MM-DD | Set up Life OS
- **Context:** Needed a structured system for AI-assisted life management
- **Decision:** Initialized Life OS with [N] projects, [N] learning topics
- **Outcome:** TBD
```

### Step 6: Confirm Boot Sequence

Read `me/boot.md` back to the user and confirm: "This is what I'll load every time we start a session. Does this look right?"

### Done

Tell the user: "Your Life OS is set up. From now on, start any session by telling me to read `me/boot.md` — or just say 'boot up' and I'll load your context. You can also ask me to add projects, log decisions, capture learning notes, or do a weekly review at any time."
