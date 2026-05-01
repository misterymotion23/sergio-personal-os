# Memory/learnings/

> Reusable lessons from experience. Things you've learned the hard way — or the good way.
> The goal: never pay the same tuition twice.

---

## When to Write Here

Write a learning entry when:
- You finish a project and have a sharp lesson to extract
- Something broke in a way that surprised you (and could happen again)
- You figured out a better way to do something recurring
- A pattern from one context turns out to apply somewhere else

**Trigger phrase:** "I'll never do that again" or "That worked better than expected."

---

## File Format

Filename: `[topic]-learning.md` (e.g., `stakeholder-alignment-learning.md`, `sprint-scoping-learning.md`)

```markdown
# Learning: [Topic]

**Date:** YYYY-MM-DD
**Source:** [Project / situation / experiment this came from]
**Tags:** #[project] #[area] #learning

## The Lesson (One Sentence)

[The sharpest possible version of what you learned]

## What Happened

[Brief context — what situation produced this insight?]

## What I'd Do Differently

[Specific, actionable: what changes next time?]

## Where This Applies

[Other contexts where this lesson is relevant]

## Connected To

- Decision: [[Memory/decisions/...]] *(if this changed how you decide something)*
- Pattern: [[Memory/patterns/...]] *(if this is a recurring dynamic)*
```

---

## Example Entry

```markdown
# Learning: Ship the Ugly Version First

**Date:** 2026-02-20
**Source:** Newsletter automation project
**Tags:** #shipping #perfectionism #learning

## The Lesson

Waiting for the "clean version" costs 3x the time and the messy version
usually teaches you what the clean version should actually be.

## What Happened

Spent 3 weeks redesigning the automation pipeline architecture before shipping.
The shipped version revealed two assumptions were wrong. Wasted 2 of those weeks.

## What I'd Do Differently

Ship v0.1 within the first week to expose real constraints.
Then redesign with actual data.

## Where This Applies

Any project where I'm designing before validating. Especially writing, product,
and automation work where the output is hard to predict in advance.
```
