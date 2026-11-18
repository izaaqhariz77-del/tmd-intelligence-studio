# Shared Quality Checklist

**Version:** 1.0 · 2026-11-18

Every agent output passes these checks, then its own `CHECKS.md`. Report the result at the end of the output (format below). A failed check is reported, not hidden.

## Accuracy

- [ ] Every market figure has a source and a time.
- [ ] Economic event dates and times come from the official publisher; Malaysia time conversion is correct (EST = UTC−5 from 1 Nov to 8 Mar; Malaysia = UTC+8).
- [ ] Every calculation has been redone, not copied.
- [ ] Methodology matches `guardrails.md` §4 (M5, lot follows the stop, no fixed %, no capital thresholds).
- [ ] Facts, estimates and opinions are labelled.

## Compliance

- [ ] No hard stop in `guardrails.md` §2 is breached.
- [ ] One content class, declared in the header.
- [ ] Nothing broker-related while the gate is closed; no coaching promotion while on hold.
- [ ] No claim about TMD or the owner that is not in the facts register.
- [ ] Disclaimer present where required (`guardrails.md` §8).
- [ ] No guarantee, urgency, fake scarcity or pressure.

## Audience

- [ ] Segment declared: PRIMARY, SECONDARY or General.
- [ ] SECONDARY protections applied where relevant.

## Voice and craft

- [ ] Correct voice for the channel and date (`guardrails.md` §9).
- [ ] One idea per piece. The first line carries it.
- [ ] Specific, not generic: could any trading account have posted this? If yes, sharpen it.
- [ ] No banned patterns (`BRAND/tone-of-voice.md` §5).

## Format

- [ ] Platform limits met (Threads: 500 characters per post; Instagram caption: 2,200 characters; hashtags: 5 maximum by brand rule).
- [ ] Output header complete; status is `DRAFT`.
- [ ] File saved in the agent's output folder with a dated, lowercase, hyphenated name.

## Data

- [ ] No personal data (`data-handling.md`).

## Checks block format

End every output with:

```
## Checks
Shared checklist: PASS | FAIL (list items)
Agent checks: PASS | FAIL (list items)
Needs the owner: (decisions, missing facts, or "none")
```
