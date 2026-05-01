# Memory/decisions/

> Decisions with lasting impact. Not every decision — only the ones where future-you
> will want to know *why* something was decided, not just *what* was decided.

---

## When to Write Here

Write a decision entry when:
- You made a call that others will build on (or will ask about later)
- You chose path A over path B and the reasoning matters
- You committed to something that changes your priorities or approach
- You made a trade-off you'll need to defend later

**Don't write here for:** Tactical day-to-day choices, obvious calls, or reversible experiments.

---

## File Format

Filename: `[topic]-decision.md` (e.g., `pricing-model-decision.md`, `hire-or-contract-decision.md`)

```markdown
# Decision: [Topic]

**Date:** YYYY-MM-DD
**Decider:** [You / team / stakeholder who made the call]
**Status:** Active / Superseded by [link]

## What Was Decided

[One clear sentence: what is now true that wasn't before?]

## Why

[The reasoning — what information, values, or constraints led here?]

## Alternatives Considered

- **Option A (chosen):** [Description]
- **Option B:** [Why not chosen]
- **Option C:** [Why not chosen]

## Trade-offs Accepted

[What are you giving up? What risk are you accepting?]

## How to Revisit

[Under what conditions should this decision be reconsidered?]
```

---

## Example Entry

```markdown
# Decision: Build vs Buy for Analytics

**Date:** 2026-03-15
**Decider:** Sergio (with input from engineering lead)
**Status:** Active

## What Was Decided

We will use an off-the-shelf analytics tool (PostHog) rather than building custom.

## Why

Custom analytics would require 6–8 weeks of eng time. We don't have validated
product-market fit yet. The cost of delay outweighs the benefit of customization.

## Alternatives Considered

- **Off-the-shelf (chosen):** PostHog, 2-day integration
- **Custom build:** Full control, but 6–8 weeks and significant maintenance overhead
- **No analytics for now:** Rejected — flying blind in growth phase is too risky

## Trade-offs Accepted

Less flexibility in custom event structures. Vendor dependency.

## How to Revisit

When we hit PostHog's pricing ceiling (~$X/month) or need event schemas they can't support.
```
