# Projects/

> One folder per active initiative. Each project folder is self-contained.
> When a project ships or is abandoned, move it to `_archive/`.

---

## How to Create a New Project

1. Create a folder: `Projects/[project-name]/`
2. Add a `spec.md` or `prd.md` (use `Templates/project-brief.md` as your starting point)
3. Add the project to the Active Projects table in `CLAUDE.md`
4. Add a task to `Tasks/active.md`: "Set up [project-name] folder"

---

## Recommended Project Folder Structure

```
Projects/[project-name]/
├── prd.md             ← What we're building and why (use template)
├── decisions.md       ← Decision log for this project
├── updates.md         ← Running project update log
└── research/          ← Project-specific research (if needed)
```

You don't need all of these immediately. Start with `prd.md`. Add others as the project grows.

---

## Decision Log Format (inside `decisions.md`)

```markdown
## [Topic] — YYYY-MM-DD

**Decision:** [What was decided]
**Rationale:** [Why — what was the reasoning?]
**Alternatives considered:** [What else was on the table?]
**Decider:** [Who made this call]
**Impact:** [What changes as a result]
```

---

## Project Update Format (inside `updates.md`)

```markdown
## Update — YYYY-MM-DD

**Status:** On Track / At Risk / Blocked / Shipped
**This week:**
- [What happened]
**Next week:**
- [What's planned]
**Blockers:**
- [Anything blocking progress]
```

---

## Archive

When a project is complete or abandoned:
1. Move the folder to `Projects/_archive/[project-name]/`
2. Add a final entry to `updates.md` explaining what happened
3. Run a retrospective using `Templates/project-retrospective.md`
4. Remove it from the Active Projects table in `CLAUDE.md`

---

## Current Active Projects

<!-- TODO: Maintain this list — it's how Claude knows what you're working on -->

| Project | Description | Status |
|---------|-------------|--------|
| <!-- TODO --> | <!-- one line --> | In Progress |
