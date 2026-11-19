# TMD_PROSPECT_INTELLIGENCE

Organises voluntary enquiries to THE MARKET DOCTRINE, with a human in charge of every decision.

## What it does

- Turns incoming messages into structured records (`enquiry-schema.md`).
- Categorises trading experience and maps each enquiry to PRIMARY, SECONDARY, Not in segment or Unclear.
- Records consent and the source of each enquiry.
- Lists the qualification information still missing.
- Sends every eligibility, suitability, vulnerability, coaching or broker question to a human review queue.

## When to use it

- Once a week, to organise new DOCTRINE messages.
- When an enquiry raises a sensitive question and you want it structured before you reply.

## Inputs

Enquiries the owner pastes into a session, or a private sheet the owner shares for the task. Never data stored in this repository.

## Outputs

Returned to the owner in the session, or written to the private store on request: records, missing-information lists, a human review queue, educational next-step suggestions, and identifier-free aggregates. Nothing is committed except aggregates.

## How to run it

- **Claude Code:** `/tmd-prospect-intelligence`, then paste the enquiries.
- **Any other AI assistant:** paste `AGENTS/_shared/guardrails.md`, `AGENTS/_shared/data-handling.md`, `AGENTS/TMD_PROSPECT_INTELLIGENCE/AGENT.md` and `enquiry-schema.md`, then the enquiries.

## Limits

- It never contacts anyone and never drafts outreach.
- It never decides eligibility or suitability.
- It suggests nothing commercial: coaching is on hold and broker content is blocked.

## Files

| File | Purpose |
|---|---|
| `AGENT.md` | Instructions |
| `CHECKS.md` | Agent-specific checks |
| `enquiry-schema.md` | Fields, categories, flags and what may be asked |
| `examples/01-input.md` | Three fictional enquiries |
| `examples/01-output.md` | Example output: records, flags, review queue, aggregates |
