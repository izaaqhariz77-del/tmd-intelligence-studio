# TMD_INTELLIGENCE

Audience and market-conversation research for THE MARKET DOCTRINE.

## What it does

- Profiles TMD's two audience segments separately: **PRIMARY** (experienced, active Forex/XAUUSD traders) and **SECONDARY** (traders rebuilding after losses).
- Maps their pain points in their own language, with evidence.
- Reads public market conversations for themes, questions and misconceptions.
- Turns all of that into ranked content opportunities.

## When to use it

- Before planning a week or a campaign.
- When content performance changes and you want to know why.
- When a new question keeps appearing in replies.

## Inputs

A research question, plus any of: Zernio analytics, the performance log, your own observations, public material, research notes. See `AGENT.md`.

## Outputs

Drafts in `RESEARCH/audience/`: segment profiles, pain-point maps, conversation scans and opportunity briefs. Status is always `DRAFT`.

## How to run it

- **Claude Code:** `/tmd-intelligence` followed by your question.
- **Any other AI assistant:** paste `AGENTS/_shared/guardrails.md` and `AGENTS/TMD_INTELLIGENCE/AGENT.md`, then your question and data.

## Limits

- Research only. It never contacts, lists or targets people.
- It will not invent statistics. Thin evidence produces a short answer and a measurement plan.

## Files

| File | Purpose |
|---|---|
| `AGENT.md` | Instructions |
| `CHECKS.md` | Agent-specific checks |
| `examples/01-input.md` | Example request using real campaign data |
| `examples/01-output.md` | Example output: SECONDARY profile and three opportunities |
