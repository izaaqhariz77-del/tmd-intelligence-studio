# DOCTRINE Journey and PDF Landing Page

**Agent:** TMD_MAGNET
**Created:** 2026-11-18
**Status:** DRAFT
**Class:** Community invitation
**Segment:** PRIMARY and SECONDARY, handled separately at step 3
**Voice:** Scripts: Campaign (Manglish). Landing page: Institutional (English).
**Channel / slot:** WhatsApp (owner's number); future website
**Sources:** Published Threads posts of 1, 5 and 6 Nov 2026; `AGENTS/_shared/guardrails.md` §10; `AGENTS/TMD_PROSPECT_INTELLIGENCE/enquiry-schema.md`
**Gate:** Regulatory review required for the privacy notice wording only
**Approval:** Reviewed by — · Approved by — · Date —

---

## 1. Journey map

| Step | What happens | Who acts | What the person is told | Data recorded (private store) |
|---|---|---|---|---|
| 1 | A post ends with "WhatsApp aku (link kat bio), type DOCTRINE." | — | Nothing yet | — |
| 2 | The person messages DOCTRINE. | The person | — | `received_at`, `channel`, `keyword`, `source_content` |
| 3 | Reply 1: the PDF, three optional questions, privacy notice. | Owner | What they get, how their number is used, how to stop | `request`, `notice_given`, `consent_scope` |
| 4 | The person answers (or not). | The person | — | `experience_category`, `segment`, `currently_trading`, `main_difficulty` |
| 5 | Reply 2: community link and expectations, sent whether or not they answered. | Owner | No signals, no fees, no account conditions | `status` → COMMUNITY JOINED when they join |
| 6 | Sunday webinar, 9pm, inside the community. | Owner | — | — |
| Exit | "STOP" or "BERHENTI" at any point: Reply 3, then no further contact. | Owner | Confirmation | `withdrawn` → DO NOT CONTACT |

**Changed from the current flow:** the community link no longer depends on answering the questions. The questions help fit education to the person; making them a gate adds friction without changing what anyone receives. Owner's call.

**Never in this journey:** coaching, broker names, account opening, deposits, referral links, questions about money. Questions on those go to the owner personally (see `AGENTS/TMD_PROSPECT_INTELLIGENCE/`).

**Follow-up:** if the person asked for the PDF and has not received it, one reminder. Nothing else.

## 2. Scripts (for the owner to send)

**Reply 1 — first contact**

```
Terima kasih sebab message. Ni PDF Basic to Advance: [link]

3 soalan ringkas, kalau kau selesa jawab:
1. Dah berapa lama trade? (belum mula / bawah 6 bulan / 6 bulan–2 tahun / lebih 2 tahun)
2. Sekarang tengah aktif trade, atau berhenti sekejap?
3. Apa satu benda paling susah untuk kau sekarang?

Nombor kau aku guna untuk hantar PDF dan info community je. Tak share dengan pihak lain. Nak berhenti, type STOP.
```

`[COMPLIANCE REVIEW REQUIRED]` for the last paragraph. "Tak share dengan pihak lain" is a promise: confirm it is true, including in any future broker relationship, before using it.

**Reply 2 — community link**

```
Ni link community: [link]

Bila masuk:
• Intro diri
• Buat 1 latihan seminggu
• Join webinar Ahad 9pm, atau tengok recap

Senyap 14 hari, aku keluarkan. Tempat tu untuk yang buat kerja.

Takde signal. Takde yuran. Takde syarat buka akaun.
```

**Reply 3 — opt-out**

```
Baik. Nombor kau dah keluar dari senarai aku. Takkan ada mesej lagi dari aku.
```

## 3. How the answers map to segments

| Answers | Segment | What they get |
|---|---|---|
| More than 2 years, active now | PRIMARY | Community; analysis-oriented webinar topics |
| Active before; mentions blown accounts or deep drawdown; wants discipline or risk structure | SECONDARY | Community; process topics. No recovery framing. |
| Not started, or under 6 months with no loss history | Not in segment | Community and PDF; free education only |
| No answer | Unclear | Community and PDF; nothing else is asked |

## 4. Landing page — "The Doctrine: Basic to Advance"

**Data stamp (top left, monospace):** `TMD · RESOURCE 01 · XAUUSD`

**Headline:** The Doctrine: Basic to Advance

**Subhead:** A free, structured guide to reading gold: candles, support and resistance, timeframes, and how to identify a breakout.

**Action:** Get the guide on WhatsApp — message DOCTRINE

**If you trade actively.** You already know the vocabulary. The guide is a reference for writing your method down in one place, so every trade can be checked against it.

**If you are rebuilding after a difficult run.** Start from structure, not from the next entry. The guide begins where a method begins: what the chart is telling you before you decide anything.

**What's inside**
- Candles
- Support and resistance
- Timeframes
- Identifying breakouts

**What it is not**
- Not signals.
- Not a promise of profit.
- No broker account needed to get the guide or join the community.

**After the guide:** the free community. A live webinar every Sunday at 9pm (Malaysia time), Q&A and chart review, and the journal template.

**About The Market Doctrine.** An independent trading education and market research brand. Its 60 Rules series is published free on Threads.

**Questions**
- *Is it free?* Yes.
- *Do I need a broker account?* No.
- *Will you ask me to deposit money?* No.
- *What happens to my number?* `[Privacy notice — COMPLIANCE REVIEW REQUIRED]`
- *How do I stop messages?* Reply STOP.

**Risk warning:** `BRAND/brand-identity.md` §9, long form.

**Footer (monospace):** `THE MARKET DOCTRINE · RESOURCE 01`

## 5. Design notes

- Background `#0B0B0C`; the two audience blocks on `#1A1B1E` panels, side by side on desktop, stacked on mobile.
- Serif headline in warm ivory `#F2ECDD`; sans body; monospace for the data stamp, section labels and footer.
- One champagne accent (`#C8AD7F`): a thin rule under the headline. The action button stays ivory on charcoal.
- Thin graphite rules (`#2A2B2F`) between sections. No photography. The guide cover is typographic: title in serif between two thin rules.

## 6. Misleading-promotion check

| Statement | Basis |
|---|---|
| Contents: candles, SR, timeframes, breakouts | Published 1 Nov |
| Free; Sunday 9pm webinar; Q&A; journal template | Published 1 and 6 Nov |
| No broker account needed; no deposit requested | Owner decision, 18 Nov: community has no account conditions |
| "Independent trading education and market research brand" | Owner's positioning, `guardrails.md` §1 |
| No performance, testimonials or credentials | None used |

## Checks

Shared checklist: PASS
Agent checks: PASS — voluntary, exit on every path, no money questions, no commercial or broker step.
Needs the owner: whether the community link stays conditional on the questions; review of the privacy wording; confirmation that "Tak share dengan pihak lain" is a promise TMD can keep.
