# TMD Intelligence Studio

The Market Doctrine — AI-powered research and content production workspace.

THE MARKET DOCTRINE is an independent financial research, trading education and media brand. This repository is its working library: brand rules, research notes, content drafts, campaign briefs and AI generation prompts, all in plain Markdown so it can be read and edited from a phone.

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

Full detail: `BRAND/brand-identity.md` → Claims policy.

## Working from mobile

- Everything is Markdown — editable in the GitHub mobile app or any text editor.
- Templates use short tables and checklists that render on small screens.
- No build step, no dependencies, no paid APIs.

## Unresolved decisions

- [ ] Lock final colour hex values (current values in `BRAND/visual-guidelines.md` are proposals).
- [ ] Lock typefaces (current choices are free-font proposals).
- [ ] Logo / wordmark files — create and add.
- [ ] Complete the verified facts register in `BRAND/brand-identity.md` (entity, regulatory status, founder bio).
- [ ] Define primary audience, market and languages.
- [ ] Define instruments covered.
- [ ] Legal review of disclaimers for each target market.
- [ ] Commercial model and any disclosures required (affiliate, IB, sponsorship).
- [ ] Approved research data sources.

## Status

Phase 1 — foundational structure. No website, no automation, no dependencies yet.
