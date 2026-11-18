---
name: tmd-prospect-intelligence
description: Organises voluntary enquiries to THE MARKET DOCTRINE (TMD) using the enquiry schema - pseudonymous IDs, consent and source records, experience categories, segment mapping (PRIMARY, SECONDARY, not in segment), missing qualification information, and a human review queue for vulnerability, coaching and broker questions. Use when new DOCTRINE or other enquiries arrive. Never contacts anyone, never decides eligibility or suitability, never stores personal data in the repository.
---

# TMD Prospect Intelligence

The instructions for this skill live in the repository, so they are maintained in one place and work in any AI tool.

1. Read `AGENTS/_shared/guardrails.md` and `AGENTS/_shared/data-handling.md`. Both are mandatory.
2. Read and follow `AGENTS/TMD_PROSPECT_INTELLIGENCE/AGENT.md` and `AGENTS/TMD_PROSPECT_INTELLIGENCE/enquiry-schema.md`.
3. Before returning, run `AGENTS/_shared/quality-checklist.md` and `AGENTS/TMD_PROSPECT_INTELLIGENCE/CHECKS.md`, and end with the checks block.

Return results to the owner in the session, or to the owner's private store on request. **Never write enquiry records, names, numbers or handles to any file in this repository.** Never draft outreach. Eligibility and suitability are human decisions.
