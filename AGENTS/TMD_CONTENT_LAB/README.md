# TMD_CONTENT_LAB

Content drafting for THE MARKET DOCTRINE.

## What it does

- Threads posts in the campaign voice (Manglish) or institutional English.
- Instagram carousels and captions, with visual notes in TMD's research-terminal style.
- Educational XAUUSD explainers.
- Trading psychology pieces.

Natural, specific, non-generic writing, checked against TMD's method and claims rules.

## When to use it

- Filling the next days of the 60 Rules queue.
- Turning a TMD_INTELLIGENCE opportunity into posts.
- Writing a pre-release briefing for a major data day.

## Inputs

A brief: channel and slot, voice, segment, class, core idea. Optional: an opportunity brief or research note. See `AGENT.md`.

## Outputs

Drafts in `CONTENT/<channel>/` with exact character counts and a checks block. Status is always `DRAFT`. It never schedules or publishes.

## How to run it

- **Claude Code:** `/tmd-content-lab` followed by the brief.
- **Any other AI assistant:** paste `AGENTS/_shared/guardrails.md`, `AGENTS/TMD_CONTENT_LAB/AGENT.md` and the voice file, then the brief.

## Limits

- No commercial, coaching or broker-related content while those are held or gated.
- It will not write the owner's personal trades or stories without real material from the owner.

## Files

| File | Purpose |
|---|---|
| `AGENT.md` | Instructions |
| `CHECKS.md` | Agent-specific checks |
| `examples/01-input.md` / `01-output.md` | Threads, campaign Manglish: a draft for Rule #30 |
| `examples/02-input.md` / `02-output.md` | Instagram, institutional English: a pre-release briefing on PCE |
