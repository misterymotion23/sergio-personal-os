# CLAUDE.md — [Your Name]'s Personal OS

> This is your AI instruction set. Fill in every `<!-- TODO -->` to make this system yours.
> Claude reads this file first in every session. The more specific you are, the better the output.

---

## Who I Am

<!-- TODO: Describe yourself honestly. This shapes every response Claude gives you. -->
<!-- Example: "I'm a Senior PM at [Company], 2 years in role, leading the growth team." -->

**Name:** <!-- TODO: Your name -->
**Role:** <!-- TODO: Your professional title and context -->
**What I care about most:** <!-- TODO: One sentence — your purpose or north star -->

**How I think:**
<!-- TODO: Pick 2–3 that fit you, or write your own -->
- <!-- e.g., Drawn to messy, unsolved problems -->
- <!-- e.g., Over-communicates with stakeholders; clarity over brevity -->
- <!-- e.g., Builder mindset — I learn by making things -->

**What energizes me:** <!-- TODO -->
**What drains me:** <!-- TODO -->

---

## What This System Does

My Personal OS helps me:

1. **Stay on top of work** — one place for projects, tasks, and decisions
2. **Think better** — Claude as a thinking partner, not just a task runner
3. **Compound knowledge** — capture what I learn so it's usable again

---

## System Map

```
├── CLAUDE.md           ← You are here. Claude reads this first.
├── GOALS.md            ← My identity, priorities, and success metrics
├── ROUTING.md          ← Where to look for what (context decision map)
├── Tasks/
│   ├── active.md       ← Current sprint (keep under 10 items)
│   └── backlog.md      ← Brain dump of future work
├── Projects/           ← Active initiatives with specs and decisions
├── Memory/
│   ├── decisions/      ← Decisions with lasting impact
│   ├── learnings/      ← Reusable lessons from experience
│   ├── patterns/       ← Recurring dynamics I've named
│   └── people/         ← Stakeholder context and relationship notes
├── Knowledge/
│   ├── research/       ← Research outputs and synthesis
│   └── reference/      ← Reference materials and domain knowledge
├── Templates/          ← Reusable formats (check here before creating)
├── _Registry/          ← Tags, tools, and integrations catalog
└── _temp/              ← Raw notes inbox (process, don't store here)
```

---

## Context Loading Rules

Claude should load context in this order depending on the task:

| If you're doing... | Load first | Then check |
|---|---|---|
| Project work | `Projects/[name]/` | `Tasks/active.md` |
| Morning planning | `Tasks/active.md` | `GOALS.md` |
| Decision-making | `GOALS.md` | `Memory/decisions/` |
| Writing to someone | `Memory/people/[name].md` | `Projects/` if applicable |
| Research or synthesis | Use sub-agent | Store in `Knowledge/research/` |
| End of week | `Tasks/active.md` | All active `Projects/`, `GOALS.md` |
| Making sense of notes | `_temp/` | `GOALS.md` for relevance filter |

**Sprint mode (fast, focused):** Only load `Tasks/active.md` + one project folder. Skip Memory.

**Deep work mode (thinking, planning):** Load `GOALS.md` + `Memory/decisions/` + `Memory/learnings/`.

**Use a sub-agent when:** Task requires 3+ web searches, heavy synthesis, or would consume more than ~10% of context. Say "spin up" or "delegate this."

---

## Key Commands

<!-- TODO: Define what each command does for you. These are your trigger phrases. -->

| Say this | What Claude does |
|---|---|
| "standup" | Morning briefing: tasks, blockers, top priority |
| "weekly update" | End-of-week: review, reflection, status draft |
| "process notes" | Route raw `_temp/` content to the right folders |
| "what should I work on" | Priority recommendation based on goals |
| <!-- TODO: add yours --> | <!-- TODO: define it --> |

---

## Operating Principles

<!-- TODO: Adjust these to match how you actually want to work -->

- **Structured over prose** — bullets, tables, and templates beat paragraphs for work output
- **Reuse before creating** — always check `Templates/` before drafting anything new
- **Write to Memory** — if a lesson, decision, or pattern could matter again, save it
- **Protect context** — never load entire folders; pull only what the task needs
- **Propose upgrades** — if a behavior repeats 3+ times, propose a Memory entry or new command

---

## Output Rules

<!-- TODO: Tell Claude how you want to receive information. These defaults work well. -->

- Concise, structured, actionable — always
- Bullets for 3+ items; prose for 1–2
- Bold key phrases in documents
- End every section with a clear recommendation or next step
- When uncertain, ask one clarifying question at a time — never five

---

## Learning Loop

| Trigger | Where to write |
|---|---|
| A decision with lasting impact | `Memory/decisions/[topic].md` |
| A reusable lesson from a project | `Memory/learnings/[topic].md` |
| A recurring dynamic I keep noticing | `Memory/patterns/[name].md` |
| A meaningful meeting or interaction | `Memory/people/[name].md` |
| A skill or command that keeps failing | Note it in `_feedback/` |

---

## System Health

Audit your OS when any of these are true:

- You keep explaining the same context to Claude that it "should already know"
- `_temp/` is always full and never gets processed
- Tasks roll over week after week without progress
- You're creating new tools instead of using the ones already here
- You haven't updated `GOALS.md` in over a month

> **Rule of thumb:** If you find yourself repeating something to Claude, write it down here.
