# TMD_MAGNET

Educational resources, voluntary enquiry journeys and landing page content for THE MARKET DOCTRINE.

## What it does

- Outlines and drafts free educational resources (guides, checklists, templates).
- Maps voluntary journeys: from a post, to a resource, to the free community, with an exit at every step.
- Writes the reply scripts the owner sends at each step.
- Writes landing page copy and design notes in TMD's research-terminal style.

## When to use it

- Creating or revising a free resource.
- Tidying the DOCTRINE WhatsApp flow.
- Preparing landing page copy for a future site.

## Inputs

A brief: the resource or journey, the segment(s), the entry point. See `AGENT.md`.

## Outputs

Drafts in `RESOURCES/`. Consent and privacy wording is marked for compliance review. Status is always `DRAFT`.

## How to run it

- **Claude Code:** `/tmd-magnet` followed by the brief.
- **Any other AI assistant:** paste `AGENTS/_shared/guardrails.md`, `AGENTS/_shared/data-handling.md` and `AGENTS/TMD_MAGNET/AGENT.md`, then the brief.

## Limits

- No coaching, broker, account or deposit steps while those are held or gated.
- It never sends messages or sets up automation. Scripts are for the owner.
- Landing pages are copy only; no website is built.

## Files

| File | Purpose |
|---|---|
| `AGENT.md` | Instructions |
| `CHECKS.md` | Agent-specific checks |
| `examples/01-input.md` | Example request: the DOCTRINE journey and a landing page for the free PDF |
| `examples/01-output.md` | Example output: journey map, scripts, landing copy, design notes |
