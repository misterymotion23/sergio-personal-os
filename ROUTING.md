# ROUTING.md — Context Decision Map

> This file reduces cognitive load. Before starting any task, use this map to know
> exactly where to look and what to load. Less context waste. Better output from Claude.
>
> Rule of thumb: **If you're about to repeat yourself to Claude, you should've written it down.**

---

## By Task Type

| If the task is... | Load first | Then check | Command |
|---|---|---|---|
| Project-specific work | `Projects/[name]/` | `Tasks/active.md` | — |
| Morning planning | `Tasks/active.md` | `GOALS.md` | `standup` |
| End of week | `Tasks/active.md` | All active `Projects/`, `GOALS.md` | `weekly update` |
| Making a decision | `GOALS.md` | `Memory/decisions/` | — |
| Research or synthesis | Use sub-agent | Store in `Knowledge/research/` | `spin up` |
| Writing to someone | `Memory/people/[name].md` | `Projects/` if applicable | `draft message` |
| Logging a meeting | Raw notes → `_temp/` | `Memory/people/[name].md` | `process notes` |
| Noticing a pattern | `Memory/patterns/` | `Memory/learnings/` | — |
| Raw notes to process | `_temp/` folder | `GOALS.md` for relevance filter | `process notes` |

---

## By Urgency

**Sprint mode (fast, focused):**
→ Only load `Tasks/active.md` + the one project folder you're in
→ Don't pull Memory unless explicitly drafting or deciding

**Deep work mode (thinking, planning):**
→ Load `GOALS.md` + `Memory/decisions/` + `Memory/learnings/`
→ Cross-project thinking needs cross-project memory

**Communication mode (drafting messages):**
→ Always start with `Memory/people/[name].md`
→ Never draft blind — even one line of context changes the tone

---

## Sub-Agent Trigger Checklist

Use a sub-agent (say "spin up" or "delegate this") when any of these are true:

- [ ] The task requires 3+ web searches
- [ ] The task is "analyze + summarize + draft" — break it into steps first
- [ ] Loading full context for the task would eat more than ~10% of context window
- [ ] The task is exploratory and might produce noise before signal

---

## Memory Write Triggers

Add to `Memory/` when any of these happen:

| Trigger | Where to write |
|---|---|
| "I'll never do that again" / "that was the wrong call" | `Memory/learnings/[topic].md` |
| "We decided to..." (lasting impact, not obvious) | `Memory/decisions/[topic].md` |
| "This keeps happening" — third time you notice something | `Memory/patterns/[name].md` |
| Meaningful 1:1 or stakeholder meeting | `Memory/people/[name].md` |

---

## File Ownership Quick Reference

| Content type | Lives in | Rule |
|---|---|---|
| Current sprint | `Tasks/active.md` | Max 10 items |
| Future work | `Tasks/backlog.md` | Everything not yet active |
| People context | `Memory/people/[name].md` | Update after every meaningful interaction |
| Decisions | `Memory/decisions/[topic].md` | Log any decision with lasting impact |
| Lessons | `Memory/learnings/[topic].md` | Capture reusable lessons |
| Recurring dynamics | `Memory/patterns/[name].md` | Name things you keep noticing |
| Research outputs | `Knowledge/research/` | Never in `_temp/` long-term |
| Reference materials | `Knowledge/reference/` | External docs, frameworks, guides |
| Raw notes in transit | `_temp/` | Process via `process notes`; don't let it accumulate |
| Project specs + decisions | `Projects/[name]/` | One folder per initiative |
| Completed projects | `Projects/_archive/` | Move when shipped or abandoned |
