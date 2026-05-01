# MCPs (Model Context Protocol Integrations)

> MCP servers extend Claude's capabilities by connecting to external tools and data sources.
> This file catalogs what's connected, what each integration does, and how to use it.

---

## What Are MCPs?

MCPs let Claude interact directly with tools like Notion, Google Calendar, Gmail, and more —
reading data and taking actions without you copying and pasting between windows.

---

## Active Integrations

<!-- TODO: List the MCPs you've enabled. Remove rows for tools you don't use. -->

| Integration | What It Does | Trigger Phrases |
|-------------|--------------|-----------------|
| <!-- e.g., Notion --> | <!-- e.g., Read/write Notion databases --> | <!-- e.g., "sync notion", "check my tasks in Notion" --> |
| <!-- e.g., Google Calendar --> | <!-- e.g., Read calendar events --> | <!-- e.g., "what's on my calendar today" --> |
| <!-- e.g., Gmail --> | <!-- e.g., Search and draft emails --> | <!-- e.g., "find that email from Sarah", "draft a reply to..." --> |
| <!-- e.g., GitHub --> | <!-- e.g., Read repos, PRs, issues --> | <!-- e.g., "what's open in that repo" --> |

---

## Canonical Data Sources

<!-- When the same data exists in multiple places, define which source wins -->

| Data Type | Canonical Source | Sync Notes |
|-----------|-----------------|------------|
| <!-- e.g., People / contacts --> | <!-- e.g., Notion Networking DB --> | <!-- e.g., Use /sync-notion to pull into Memory/people/ --> |
| <!-- e.g., Meeting notes --> | <!-- e.g., This OS → _temp/ → Memory/ --> | <!-- e.g., Use "process notes" to route --> |
| <!-- e.g., Tasks --> | <!-- Tasks/active.md --> | <!-- Sync from external tools weekly --> |

---

## How to Add a New MCP

1. Enable the MCP in Claude Code settings
2. Test it with a simple query
3. Add it to the Active Integrations table above
4. Add a trigger phrase to your `CLAUDE.md` Key Commands section
5. Document the canonical data source if relevant

---

<!-- TODO: Update this file whenever you add or remove an MCP integration. -->
