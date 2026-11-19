# Output Header

**Version:** 1.0 · 2026-11-18

Every file an agent produces starts with this block, in the same bold-key style as `TEMPLATES/`.

```
# [Title]

**Agent:** TMD_INTELLIGENCE | TMD_AUTHORITY | TMD_CONTENT_LAB | TMD_MAGNET | TMD_PROSPECT_INTELLIGENCE
**Created:** YYYY-MM-DD
**Status:** DRAFT
**Class:** Educational | Community invitation | Commercial | Broker-related | Research (internal)
**Segment:** PRIMARY | SECONDARY | General
**Voice:** Campaign (Manglish) | Institutional (English) | n/a
**Channel / slot:** e.g. Threads, Sun 29 Nov 8:30am MYT | n/a
**Sources:** files, URLs and data used, with dates
**Gate:** None | Regulatory review required | Held (reason)
**Approval:** Reviewed by — · Approved by — · Date —
```

## Rules

- `Status` starts at `DRAFT`. Only the owner changes it (`approval-workflow.md`).
- `Sources` lists everything the output relies on. "General knowledge" is not a source for figures or dates.
- `Gate` must say `Regulatory review required` for anything broker-related, or for disclosure, consent or risk-warning wording.

## File naming

Lowercase, hyphenated, date first: `YYYY-MM-DD-topic-slug.md`. Save in the agent's output folder:

| Agent | Folder |
|---|---|
| TMD_INTELLIGENCE | `RESEARCH/audience/` |
| TMD_AUTHORITY | `STRATEGY/` |
| TMD_CONTENT_LAB | `CONTENT/<channel>/` |
| TMD_MAGNET | `RESOURCES/` |
| TMD_PROSPECT_INTELLIGENCE | Not saved in this repository |

## Footer

Every file ends with the checks block from `quality-checklist.md`.
