# Optional Integrations

**Version:** 1.0 · 2026-11-18

Every agent works with no integrations at all: give it files and text, get drafts back. Connectors make some steps faster. None is required, none is paid for by default, and none may act without the owner's instruction.

**No API keys, tokens or passwords are ever written into this repository.** Connectors authenticate through the owner's accounts outside the repo. If code is ever added, secrets go in environment variables or a secrets manager, and `.env` files are excluded by `.gitignore`.

| Connector | Useful for | Allowed without asking | Needs the owner's explicit instruction | Never |
|---|---|---|---|---|
| Zernio | Threads scheduling and analytics | Read analytics; read the scheduled queue; validate a draft against platform limits | Create, edit, schedule, pause or unpublish any post | Publish without an instruction naming the item; use its paid support tool |
| Google Sheets / Drive | Private enquiry register (`data-handling.md`) | Nothing | Read a sheet the owner shares for a specific task | Copy personal data into the repository |
| Web search | Research; official sources for economic dates | Search and read public pages | — | Automated scraping; logged-in browsing of other people's content |
| Canva | Carousels and visual drafts | Read designs the owner shares | Create or edit designs; any paid feature | Use paid features without approval of the spend |
| Higgsfield | Image generation | Check cost estimates | Any generation that costs credits | Generate real, identifiable people |

## Known limits in this workspace

- Direct page fetches of some official sites (bea.gov, census.gov, nyse.com) are blocked by the session's network settings. Searches restricted to those domains work. Record which method was used.
- Threads posts cannot be edited after publication. Corrections mean unpublishing, which needs the owner's instruction.
