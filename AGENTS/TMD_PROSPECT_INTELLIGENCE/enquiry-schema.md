# Enquiry Schema

**Version:** 1.0 · 2026-11-18

The structure for organising voluntary enquiries. **Records live only in the owner's private store** (for example, a Google Sheet in the owner's account). This file defines the columns; it never holds a record.

## Fields

| Field | Required | Values | Notes |
|---|---|---|---|
| `enquiry_id` | Yes | `ENQ-YYMM-NNN` | Pseudonymous. The only identifier used in any session summary. |
| `received_at` | Yes | Date and time, Malaysia time | |
| `channel` | Yes | WhatsApp · Threads reply · Threads DM · Email · In person · Other | |
| `source_content` | If known | Post date and slot, or post URL | What prompted the enquiry |
| `keyword` | If used | DOCTRINE · COACHING · Other · None | |
| `contact_ref` | Yes | — | **Private store only.** Never copied into a session summary or this repository. |
| `request` | Yes | PDF · Community · Webinar · Question · Coaching · Broker or account · Other | What the person asked for, in their terms |
| `experience_category` | After triage | E0 · E1 · E2 · E3 · Unknown | See definitions below |
| `segment` | After triage | PRIMARY · SECONDARY · Not in segment · Unclear | See mapping below |
| `currently_trading` | If known | Yes · No · Unknown | |
| `main_difficulty` | Optional | Short paraphrase | Never a direct quote that identifies the person |
| `consent_scope` | Before any reply beyond the item requested | What the person agreed to receive, and how | e.g. "PDF and community information by WhatsApp" |
| `consent_date` | With consent | Date | |
| `notice_given` | Yes | Yes · No, with date | Privacy notice at first contact |
| `withdrawn` | Yes | No · Yes, with date | Yes means DO NOT CONTACT |
| `missing_info` | Generated | List | Qualification information not yet known |
| `flags` | Generated | VULNERABILITY · BROKER-GATE · COACHING-HOLD · OTHER | See flags below |
| `human_review` | Generated | No · Yes, with reason | |
| `reviewer` / `review_date` / `decision` | Human only | — | Never filled in by an agent |
| `status` | Yes | NEW · AWAITING INFO · HUMAN REVIEW · RESPONDED · COMMUNITY JOINED · CLOSED · DO NOT CONTACT | |
| `retention_until` | Yes | Date | Set by the owner's retention policy (open decision; proposal in `RESOURCES/2026-11-18-journey-doctrine-privacy-and-retention.md`) |

## Experience categories

Default heuristics. The owner may adjust the thresholds.

| Code | Description |
|---|---|
| E0 | Not trading yet |
| E1 | New: under 6 months live, or no consistent method |
| E2 | Developing: 6 months to 2 years, has a method, execution inconsistent |
| E3 | Experienced: 2+ years live with a defined method; understands leverage and drawdown |

## Segment mapping

| Segment | Rule |
|---|---|
| PRIMARY | E3 and currently trading |
| SECONDARY | Was active (E1–E3), reports significant drawdown or blown accounts, wants to rebuild discipline, risk management or execution |
| Not in segment | E0, or E1 with no loss history. Free education only. |
| Unclear | Not enough information. Ask only the minimum, or leave it. |

## Flags

| Flag | Raised when | Consequence |
|---|---|---|
| VULNERABILITY | Mentions borrowing to trade, debt, distress, urgency to win back losses, or gambling-like language; or signs the person may be under 18 | Human review. No commercial suggestion of any kind. |
| BROKER-GATE | Asks about a broker, opening an account, deposits, account types or leverage | Human review. The gate is closed (`guardrails.md` §6). |
| COACHING-HOLD | Asks about coaching | Human review. Coaching promotion is on hold. |
| OTHER | Anything the agent cannot classify safely | Human review |

## Qualification information

| Category | Examples | Who may ask |
|---|---|---|
| Education fit | Experience, currently trading, instruments, main difficulty | Scripts (TMD_MAGNET) and the owner |
| Never asked | Balance, deposit amount, income, debts, broker account details, logins | Nobody |
| Regulatory eligibility and suitability | Age, country of residence, any regulator or broker requirement | **The owner only, and only if the broker gate opens.** An agent never assesses or decides these. |
