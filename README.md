# Personal OS — Starter Kit

**An AI-native personal operating system for Claude Code**

---

## What Is This?

Most professionals use 5+ disconnected tools with no connecting logic. Notes live in one place, tasks in another, decisions nowhere. Context gets lost. Work repeats.

A **Personal OS** solves this by giving you — and your AI assistant — a single structured workspace. Not just a folder system: a thinking environment where work, decisions, and knowledge compound over time.

This starter kit is the architecture. You fill it in.

> Built as part of the [**Master Personal System OS**](https://sergio-martinez.com) course by Sergio Martinez. Inspired by [amanai personal OS](https://github.com/amanaiproduct/personal-os) and [carls-product-os](https://github.com/carlvellotti/carls-product-os) 

---

## Structure

```
[your-name]-os/
├── CLAUDE.md           ← AI instruction set. Claude reads this first, every session.
├── GOALS.md            ← Your identity, what you own, and quarterly goals
├── ROUTING.md          ← Context decision map: what to load and when
├── Tasks/
│   ├── active.md       ← Current sprint (keep under 10 items)
│   └── backlog.md      ← Brain dump of future work
├── Projects/           ← One folder per active initiative
├── Memory/
│   ├── decisions/      ← Decisions with lasting impact
│   ├── learnings/      ← Reusable lessons from experience
│   ├── patterns/       ← Recurring dynamics you've named
│   └── people/         ← Stakeholder context and relationship notes
├── Knowledge/
│   ├── research/       ← Research outputs and synthesis
│   └── reference/      ← Reference materials and domain knowledge
├── Templates/          ← Reusable document formats
├── _Registry/          ← Tags, tools, and integrations catalog
└── _temp/              ← Raw notes inbox (process, don't store)
```

---

## Key Concepts

### CLAUDE.md is the nerve center

Every session, Claude reads `CLAUDE.md` first. This is where you define who you are, how you like to work, and what context rules to follow. The more specific you are here, the better every output becomes.

### Memory compounds your knowledge

Most AI interactions start from zero. The `Memory/` system changes that:

- `decisions/` — *why* you made past calls, so future decisions build on them
- `learnings/` — lessons extracted from real work, so you don't pay the same tuition twice
- `patterns/` — recurring dynamics you've named, so you can recognize them early
- `people/` — stakeholder context, so you never draft a message blind

### ROUTING.md reduces friction

Before any session, `ROUTING.md` tells Claude exactly what to load for the task at hand — sprint work, deep thinking, communication, or research. Less context waste. Better output.

### Templates over invention

Six templates cover the most common work artifacts: project briefs, 1:1 notes, weekly updates, research summaries, decision logs, and retrospectives. Use them. Don't reinvent formats from scratch.

---

## Getting Started

**Step 1 — Copy this folder**
Rename it to `[your-name]-os/` and open it in Claude Code.

**Step 2 — Fill in the two most important files**
Open `CLAUDE.md` and `GOALS.md`. Fill in every `<!-- TODO -->`. These two files give you 80% of the value.

**Step 3 — Add your first real work**
Add a task to `Tasks/active.md`. Create your first project folder under `Projects/`.

**Step 4 — Let the system grow**
Don't over-engineer upfront. Add `Memory/` entries as decisions and lessons happen naturally. Add custom commands to `CLAUDE.md` when you notice repeated patterns.

---

## File Ownership Rules

| Content type | Lives in | Rule |
| --- | --- | --- |
| Current sprint | `Tasks/active.md` | Max 10 items |
| Future work | `Tasks/backlog.md` | Everything not yet active |
| People context | `Memory/people/[name].md` | Update after meaningful interactions |
| Decisions | `Memory/decisions/[topic].md` | Log decisions with lasting impact |
| Lessons | `Memory/learnings/[topic].md` | Capture reusable lessons |
| Raw notes | `_temp/` | Process regularly — don't let it accumulate |

---

## The Three Laws of a Working OS

**1. If it's not in here, it doesn't exist.**
The system only works if you use it.

**2. Capture first, organize second.**
Drop everything in `_temp/` or `Tasks/backlog.md`. Don't let perfect organization block fast capture.

**3. The system serves you — not the other way around.**
Remove folders you don't use. Simplify templates that feel like busywork. Start minimal, add structure when you feel friction.

---

## About

Built by **Sergio Martinez** — digital strategist, design leader, and educator.

- **Course:** Master Personal System OS *(link coming soon)*
- **LinkedIn:** [linkedin.com/in/sergiomartinez](https://linkedin.com/in/sergiomartinez)
