# Data Handling

**Version:** 1.0 · 2026-11-18

## What counts as personal data

Names, usernames and handles, phone numbers, email addresses, photos, locations, messages, and any trading details (balances, losses, account numbers) that can be tied to a person.

## Never in this repository

- Real enquiries, contact details or message threads.
- Screenshots of chats, comments or DMs.
- Usernames of people who reply to posts.
- Any balance, loss or personal story that could identify someone.

Git history is permanent and the repository is stored on GitHub. Deleting a file later does not remove it from history.

## Where real records live

In a private store the owner controls, such as a Google Sheet in the owner's account with access limited to the owner. Records are entered by a person, not by an automated process.

Agents work on real records only when the owner pastes them into a session or shares the private store for that task. Outputs use pseudonymous IDs (`ENQ-YYMM-NNN`) and are returned to the owner, not committed.

## Consent

- Record what the person asked for, what they agreed to, how and when (`AGENTS/TMD_PROSPECT_INTELLIGENCE/enquiry-schema.md`).
- Use data only for the purpose the person agreed to.
- "STOP", "BERHENTI" or any clear refusal means do not contact again. Record it.
- Give a short privacy notice at first contact (wording drafted by TMD_MAGNET, subject to review).

## Public conversations

- Record themes, not people. Paraphrase; do not quote anything long enough to identify the author.
- Public sources only. No scraping, automated collection or logged-in browsing of other people's content.
- Respect each platform's terms.

## Retention

Keep records only as long as needed for the purpose. The owner sets the retention period (open decision) and deletes records after it.

## Legal note

Malaysia's Personal Data Protection Act 2010 is likely to apply to enquiry records (consent, notice and choice, disclosure, security, retention, data integrity, access). This is a flag, not legal advice. The owner should confirm obligations with a qualified adviser.

## If personal data is found in the repository

Stop. Do not commit. Tell the owner. If it was already committed, removing it from history is the owner's decision and needs care.

## Safety net

`.gitignore` excludes `PROSPECTS/private/`. This is a guard against accidents, not a storage location: anything saved there exists only on the machine where it was saved.
