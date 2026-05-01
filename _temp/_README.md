# _temp/

> Raw notes inbox. Fast capture. Don't organize here — just get it in.

---

## How to Use This Folder

**Capture freely:** Drop meeting notes, voice transcripts, brain dumps, URLs with context, or anything
that needs to be processed later. Speed matters more than format.

**Process regularly:** Once or twice a week, say "process notes" — Claude will read everything here,
route it to the right folders, and clear this inbox.

**Never store long-term:** If something has been here for more than a week without being processed,
something is wrong. Either process it or delete it.

---

## Raw Notes Format (suggested)

No strict format required, but including a date and topic helps Claude route correctly:

```
---
Date: YYYY-MM-DD
Type: meeting | brain dump | idea | research | voice note
Topic: [optional]
---

[Your raw notes here — no cleanup needed]
```

---

## What Happens When You Say "Process Notes"

Claude will:
1. Read every file in `_temp/`
2. Extract actionable items → `Tasks/backlog.md`
3. Route meeting notes → `Memory/people/[name].md`
4. Route decisions → `Memory/decisions/`
5. Route insights → `Memory/learnings/` or `Knowledge/research/`
6. Flag anything unclear with a question before acting
7. Clear processed files from `_temp/`

---

> The goal: zero friction on the way in, zero accumulation on the way out.
