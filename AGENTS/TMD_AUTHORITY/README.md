# TMD_AUTHORITY

Positioning, thought leadership and brand consistency for THE MARKET DOCTRINE.

## What it does

- Writes TMD's positioning for each audience segment, using only claims TMD can prove today.
- Defines the thought-leadership pillars TMD actually holds in its published content.
- Reviews drafts, weeks of posts or pages for consistency with the brand, voice, claims policy and method.
- Proposes changes to `BRAND/`, which the owner decides on.

## When to use it

- Before a new campaign, resource or landing page.
- When content starts to drift in voice or claims.
- When you want to know what TMD can and cannot say about itself.

## Inputs

A positioning question, or the item(s) to review. See `AGENT.md`.

## Outputs

Drafts in `STRATEGY/`: positioning statements, pillars, proof inventories, consistency reviews. Status is always `DRAFT`. It never edits `BRAND/` directly.

## How to run it

- **Claude Code:** `/tmd-authority` followed by the task.
- **Any other AI assistant:** paste `AGENTS/_shared/guardrails.md` and `AGENTS/TMD_AUTHORITY/AGENT.md`, then the task.

## Limits

- It cannot create credibility the facts register does not support. Gaps are listed, not filled.

## Files

| File | Purpose |
|---|---|
| `AGENT.md` | Instructions |
| `CHECKS.md` | Agent-specific checks |
| `examples/01-input.md` | Example request: PRIMARY positioning |
| `examples/01-output.md` | Example output: statement, pillars, proof inventory, consistency findings |
