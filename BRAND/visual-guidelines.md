# Visual Guidelines — THE MARKET DOCTRINE

> How TMD looks. The reference point is an editorial financial research publication, not a trading signal page.

## 1. Visual direction

- Deep charcoal and black foundations.
- Warm ivory typography.
- Restrained champagne gold as an accent only.
- Editorial financial research aesthetic.
- Premium cinematic photography.

If a design feels loud, remove something.

## 2. Colour palette

> Hex values below are **proposed starting points**, not final. Confirm and lock them (see README → unresolved decisions).

| Role | Name | Hex (proposed) | Use |
|---|---|---|---|
| Primary background | Black | `#0B0B0C` | Main canvas |
| Secondary background | Deep Charcoal | `#1A1B1E` | Cards, panels, alternating slides |
| Divider / subtle | Graphite | `#2A2B2F` | Rules, borders, chart grid |
| Primary text | Warm Ivory | `#F2ECDD` | Headlines and body |
| Secondary text | Muted Ivory | `#B9B2A3` | Captions, labels, footers |
| Accent | Champagne Gold | `#C8AD7F` | Thin rules, one key word, logo mark |

**Usage ratio:** roughly 70% black/charcoal, 25% ivory, 5% gold or less.

**Gold rules**
- One gold element per frame. Never gold body text.
- No gradients, glows, metallic or foil effects.

**Chart colours**
- Avoid bright red/green. Use ivory for the main series, muted ivory for secondary, gold for the single highlighted level or point.

## 3. Typography

> Typefaces are **proposed**, chosen because they are free and available in Canva and Google Fonts. Confirm before locking.

| Role | Proposed typeface | Notes |
|---|---|---|
| Headlines | Editorial serif (e.g. Playfair Display or Cormorant Garamond) | Sentence case or all caps with wide tracking |
| Body / UI | Clean sans (e.g. Inter) | Regular weight; avoid bold stacks |
| Data / labels | Monospace or tabular sans (e.g. IBM Plex Mono) | Prices, dates, tickers |

Rules:
- Maximum two typefaces per asset.
- Generous line spacing and margins. White space (black space) is part of the brand.
- No outlines, drop shadows or warped text.

## 4. Layout

- Strong grid, left-aligned text by default.
- Wide margins: keep content inside ~10% safe area on every edge.
- One focal point per frame.
- Thin gold or graphite rule to separate header from body.
- Footer: small `THE MARKET DOCTRINE` wordmark + date or issue label.

### Format sizes

| Format | Size (px) | Ratio |
|---|---|---|
| Instagram post / carousel | 1080 × 1350 | 4:5 |
| Instagram story / Reel / TikTok | 1080 × 1920 | 9:16 |
| Threads image | 1080 × 1350 | 4:5 |
| WhatsApp broadcast image | 1080 × 1080 | 1:1 |

For 9:16 video, keep text clear of the top ~250 px and bottom ~400 px (platform UI overlap).

## 5. Photography and imagery

**Look**
- Cinematic, low-key lighting. Deep shadows, soft directional light.
- Muted, desaturated colour with warm highlights.
- Shallow depth of field, subtle film grain.

**Subjects that fit**
- Architecture: financial districts, stone, glass, steel.
- Desks, documents, newspapers, terminals shown out of focus.
- Materials: gold bullion shot soberly, paper, leather, brass.
- Cityscapes at dusk or night, weather, long exposure.
- Anonymous human presence: hands, silhouettes, figures from behind.

**Never**
- Supercars, private jets, cash stacks, watches as flex, beach laptops.
- Rocket, moon, fire or money emoji graphics.
- Neon green/red candlestick walls.
- Fake account screenshots or fabricated P&L.
- AI-generated faces presented as real analysts, clients or staff.
- Real logos of banks, brokers, exchanges or media outlets implying affiliation.

## 6. AI image and video generation (Higgsfield)

Reusable style block — append to prompts and adjust the subject:

```
Cinematic editorial photograph, low-key lighting, deep charcoal and black
tones, warm ivory highlights, restrained champagne gold accent, shallow depth
of field, subtle film grain, 35mm look, premium financial research magazine
aesthetic, minimal composition, negative space for text.
```

Negative block:

```
No text, no logos, no watermarks, no neon, no bright red or green, no cash,
no luxury cars, no cartoon style, no oversaturated colour, no distorted hands
or faces.
```

Rules:
- Generate imagery without embedded text; add typography afterwards in the design tool.
- Do not generate real, identifiable people.
- Save prompts that work in `HIGGSFIELD/image-prompts/` and `HIGGSFIELD/video-prompts/` (see README for naming).

**Video motion:** slow push-ins, slow pans, locked-off shots. No fast cuts, shake or flashy transitions.

## 7. Logo

- Logo files: _not yet created / not yet added to this repo._
- Interim: set `THE MARKET DOCTRINE` in the headline serif, all caps, wide letter-spacing, warm ivory on black.
- Do not improvise new logo marks per post.

## 8. Pre-publish visual checklist

- [ ] Background is black or charcoal?
- [ ] Gold used once, sparingly?
- [ ] Maximum two typefaces?
- [ ] Text readable on a phone at arm's length?
- [ ] No hype imagery, no fake screenshots, no implied affiliations?
- [ ] Wordmark and date/issue label present?
