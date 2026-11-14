# TMD Intelligence Studio

The Market Doctrine — AI-powered research and content production workspace.

THE MARKET DOCTRINE is an independent financial research and trading education media brand that also operates as a transparently disclosed acquisition channel for its Introducing Broker business. It is not a pure media company.

Three pillars:

1. Independent financial research and market intelligence.
2. Trading education and methodology.
3. Transparent, voluntary Introducing Broker acquisition.

Positioning is research-first and education-first, never aggressive broker promotion.

This repository is its working library: brand rules, research notes, content drafts, campaign briefs and AI generation prompts, all in plain Markdown so it can be read and edited from a phone.

## Folder structure

```
tmd-intelligence-studio/
├── README.md
├── BRAND/
│   ├── brand-identity.md        What the brand is, claims policy, disclaimers
│   ├── tone-of-voice.md         How we write, banned patterns, checklist
│   └── visual-guidelines.md     Colour, type, imagery, AI style blocks
├── RESEARCH/
│   ├── daily-market-research/   One dated note per day
│   └── macro-library/           Evergreen macro reference notes
├── CONTENT/
│   ├── threads/
│   ├── instagram/
│   ├── tiktok/
│   └── whatsapp/
├── CAMPAIGNS/                   One brief per campaign
├── HIGGSFIELD/
│   ├── image-prompts/           Saved image prompts that work
│   └── video-prompts/           Saved video prompts that work
└── TEMPLATES/
    ├── market-research-template.md
    ├── daily-content-template.md
    └── campaign-brief-template.md
```

## Daily workflow

1. **Research** — copy `TEMPLATES/market-research-template.md` into `RESEARCH/daily-market-research/` and fill it in.
2. **Choose one idea** — pick the strongest content angle from the research note.
3. **Write** — copy `TEMPLATES/daily-content-template.md` and adapt the idea for each channel.
4. **Visuals** — write or reuse prompts in `HIGGSFIELD/`, following `BRAND/visual-guidelines.md`.
5. **Check** — run the pre-publish checklist in `BRAND/tone-of-voice.md`.
6. **Publish and log** — record links and performance notes in the content file.

For multi-day pushes, start with `TEMPLATES/campaign-brief-template.md` in `CAMPAIGNS/`.

## File naming

Lowercase, hyphens, date first so files sort correctly.

| Type | Pattern | Example |
|---|---|---|
| Daily research | `YYYY-MM-DD-market-research.md` | `2026-01-15-market-research.md` |
| Macro library | `topic-slug.md` | `us-interest-rates.md` |
| Content | `YYYY-MM-DD-topic-slug.md` | `2026-01-15-gold-rejects-resistance.md` |
| Campaign | `YYYY-MM-campaign-name.md` | `2026-02-risk-management-series.md` |
| Higgsfield prompt | `subject-slug.md` | `trading-desk-at-dusk.md` |

## Non-negotiable rules

- No invented company history, credentials, regulatory status or performance claims.
- No guaranteed returns, exaggerated trading claims or fake financial authority.
- Facts are sourced. Opinions are labelled. Market views include an invalidation.
- Every published piece carries a disclaimer.
- Broker referral and commercial relationships are disclosed in the content itself, beside the CTA.
- TMD is never described as independent or neutral when a commercial relationship is being discussed.
- Educational and promotional content are kept distinct. A referral CTA makes the piece promotional.
- Jurisdiction-specific compliance wording is flagged `[COMPLIANCE REVIEW REQUIRED]` and reviewed before publication.

Full detail: `BRAND/brand-identity.md` → Claims policy and Commercial disclosure policy.

## Working from mobile

- Everything is Markdown — editable in the GitHub mobile app or any text editor.
- Templates use short tables and checklists that render on small screens.
- No build step, no dependencies, no paid APIs.

## Decisions

### Resolved

- [x] Commercial model — media brand plus transparently disclosed Introducing Broker acquisition channel; three pillars; research-first and education-first (decided 2026-11-14).
- [x] Disclosure principles — disclose in content, no "independent" framing around commercial relationships, educational and promotional kept distinct, jurisdiction wording reviewed before publication.

### Unresolved

Blocking promotional content:

- [ ] Record partner broker name(s), regulator(s) and licence numbers in the verified facts register.
- [ ] Record how TMD is compensated, so the long disclosure can state it.
- [ ] Define target jurisdictions and confirm the broker may accept clients there.
- [ ] Compliance review of all disclaimer and disclosure wording per jurisdiction.
- [ ] Check platform financial-promotion rules for each channel.
- [ ] Confirm the promotional content ratio (proposed: no more than 1 in 10).

General:

- [ ] Complete the rest of the verified facts register (entity, regulatory status, founder bio).
- [ ] Define primary audience and languages.
- [ ] Define instruments covered.
- [ ] Lock final colour hex values (current values in `BRAND/visual-guidelines.md` are proposals).
- [ ] Lock typefaces (current choices are free-font proposals).
- [ ] Logo / wordmark files — create and add.
- [ ] Approved research data sources.

## Status

Phase 1 — foundational structure. No website, no automation, no dependencies yet.
