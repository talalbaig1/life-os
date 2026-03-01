# Boot Sequence

When starting a new session, load these files in order:

1. **Read `me/context.md`** — Understand who you're working with
2. **Read `me/prompts/default.md`** — Load operating instructions
3. **Read `me/tools.md`** — Know what tools are available
4. **Scan `do/` folder** — List all active projects (read each README.md)
5. **Read latest entry in `log/journal/`** — Know what happened most recently
6. **Read `log/decisions.md`** (last 5 entries) — Know recent decisions

After loading, give a brief status: "Here's what I see: [N] active projects, last session was [date], your current priorities are [X, Y, Z]. What do you want to work on?"

## Session Types

If the user asks for a specific session type, also load:

- **Weekly Review** → Read all `log/journal/` entries from the past 7 days + all project READMEs
- **Project Deep Dive** → Read the specific project's full folder
- **Learning Session** → Read `learn/index.md` + the specific topic file
- **Decision Making** → Read `me/context.md` priorities + relevant project README + `log/decisions.md`
