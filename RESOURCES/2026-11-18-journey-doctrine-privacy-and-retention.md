# DOCTRINE Journey — Privacy Notice Review and Retention Proposal

**Agent:** TMD_MAGNET
**Created:** 2026-11-18
**Status:** DRAFT
**Class:** Research (internal)
**Segment:** General
**Voice:** Review in English. Proposed notice in Malay and English.
**Channel / slot:** WhatsApp (owner's number): first reply to DOCTRINE, plus a full notice linked from it
**Sources:** Reply 1 and the journey in `AGENTS/TMD_MAGNET/examples/01-output.md`; `AGENTS/_shared/data-handling.md`; `AGENTS/TMD_PROSPECT_INTELLIGENCE/enquiry-schema.md`; published community posts (5, 6 and 19 Nov); Personal Data Protection Act 2010 and the Personal Data Protection (Amendment) Act 2024, as summarised by the secondary sources listed at the end (read 18 Nov 2026). The Act text and the Commissioner's guidelines were not read directly.
**Gate:** Regulatory review required. All notice wording below is `[COMPLIANCE REVIEW REQUIRED]`.
**Approval:** Reviewed by — · Approved by — · Date —

---

> Not legal advice. This is a structured list of questions and gaps for a qualified reviewer. Section numbers are given so the reviewer can check them against the Act; where a point rests only on a secondary source, it says so.

## 1. Summary

The current notice is a good start: short, plain, with an opt-out. It does not yet cover what the Act's notice principle asks for. The gaps that matter most:

1. **It does not say the person can see, correct or delete their data, or who to contact.**
2. **"Tak share dengan pihak lain" is incomplete.** WhatsApp, Google and any webinar platform hold the data on the owner's behalf, possibly outside Malaysia.
3. **It is in Malay only.** The Act requires the notice in Malay and English.
4. **Optional or required is unclear.** The notice says the questions are optional, while published posts say "Jawab 3 soalan, aku bagi link". If the answers are a condition for the community link, the notice must say so.
5. **There is no retention rule.** Section 4 proposes one, with periods left for the owner to set after review.

## 2. Does the Act apply?

The Act covers personal data processed in respect of commercial transactions. The DOCTRINE community is free, but it sits inside a business that has offered paid coaching and has an IB commercial relationship. **Working assumption: the Act applies.** The reviewer should confirm.

Since the 2024 amendments took effect, the Act calls the person or business responsible a **data controller** (previously "data user"). The owner, or the owner's registered business, would be the data controller. `[Owner to supply: legal name or business name and contact for privacy requests]`

## 3. Review of the current notice

Current text (Reply 1, last paragraph):

```
Nombor kau aku guna untuk hantar PDF dan info community je. Tak share dengan pihak lain. Nak berhenti, type STOP.
```

Checked against the Notice and Choice Principle (s7), as summarised by the sources:

| s7 requirement | Current notice | Gap | Proposed fix |
|---|---|---|---|
| That personal data is processed, and a description of it | "Nombor kau" | Name or display name, messages and answers to the three questions are not mentioned | List them |
| Purposes | PDF and community information | Organising enquiries and fitting education to the answers are not mentioned | Add both |
| Source of the data | Not stated | Minor: the data comes from the person | One clause |
| Right to request access and correction; contact for enquiries or complaints | Missing | **Main gap** | Add rights and a contact |
| Class of third parties the data may be disclosed to | "Tak share dengan pihak lain" | Service providers hold the data; the promise may not be accurate as worded, and must stay true in any future broker relationship | Name the classes (service providers); "I don't sell your data" |
| Choices and means to limit processing | "type STOP" | Good. Add correction and deletion | Extend |
| Whether supplying the data is voluntary or obligatory | "kalau kau selesa jawab" | Conflicts with published "Jawab 3 soalan, aku bagi link" | Owner decides (section 6) |
| Consequences of not supplying, if obligatory | Not stated | Depends on the decision above | State it |
| Malay and English (s7(3) per one source; the bilingual requirement appears in several) | Malay only | **Gap** | Add English |
| Given as soon as practicable, at first collection | Yes, in Reply 1 | None | Keep |

Other principles to cover in practice, not only in the notice:

| Principle | What it means here |
|---|---|
| Disclosure (s8) | Use or disclose data only for the stated purposes. Any broker referral use would need a new notice and consent first. It is blocked anyway while the gate is closed. |
| Security (s9) | Phone screen lock; two-factor login on the WhatsApp and Google accounts; the private sheet shared with nobody; chat backups encrypted. Since 2024, data processors are also bound by this principle. |
| Retention (s10) | Keep data no longer than the purpose needs, then destroy or permanently delete it. See section 4. |
| Data integrity (s11) | Keep records accurate; correct them on request. |
| Access (s12) | Give access and corrections on request. |
| Rights the person can use | Access (s30), correction (s34), withdrawal of consent (s38), preventing processing likely to cause damage or distress (s42), preventing direct marketing (s43), and data portability (added in 2024). Section numbers to be confirmed by the reviewer. |
| Cross-border transfer (s129, amended) | WhatsApp and Google may store data outside Malaysia. The 2024 amendment removed the ministerial whitelist. Transfers are now allowed where the destination has a substantially similar law or adequate protection, or another statutory condition applies. Cross-border transfer guidelines are reported as issued 29 April 2025. |

## 4. Retention schedule (proposal)

Periods are **not set here**. Each row gives the purpose, the legal basis to be confirmed, and the event that ends the purpose. The owner sets each period after review. Where a law sets a period, the reviewer names it.

| # | Data | Where held | Purpose | Legal basis (to confirm) | Purpose ends when | Period | Disposal |
|---|---|---|---|---|---|---|---|
| 1 | Phone number, WhatsApp name, chat messages | WhatsApp on the owner's phone, plus chat backups | Answer the request; send the PDF, community link and information | Consent (s6), given by messaging DOCTRINE after the notice | The person sends STOP; or leaves or is removed from the community and no conversation is open; or the request is complete and they did not join | Owner to set | Delete the chat and contact labels. Backups keep deleted chats until they are overwritten; set the backup policy to match. |
| 2 | Enquiry record: schema fields (pseudonymous ID, dates, channel, source, keyword, request, experience category, segment, currently trading, main difficulty, flags, status) | Owner's private store, e.g. Google Sheets | Organise enquiries; fit education to the person; human review queue | Consent (s6) | Same events as row 1, or human review closed | Owner to set | Delete the row. Keep only counts with no identifiers. |
| 3 | `contact_ref` (the link from the record to the person) | Private store only | Link the record to the conversation | Consent (s6) | Same as row 2 | Same as row 2 | Delete first. Without it, the rest of the record is pseudonymous. |
| 4 | Consent and notice record: what the person agreed to, when, which notice version | Private store | Show that notice was given and consent obtained | To confirm: accountability under the Act and the Personal Data Protection Standard 2015 | As long as the data in rows 1–3 is held | Owner to set (reviewer to advise whether to keep it for a time after deletion) | Delete with or after the record |
| 5 | Opt-out record: contact reference and STOP date | Private store | Honour the opt-out; avoid contacting the person again | Compliance with the person's request (s38, s43) | Needed only while any contact list exists that could reach them. The journey sends nothing unprompted, so this may not be needed at all. | Owner to set, or not kept | Delete when no list exists |
| 6 | Community membership | WhatsApp community or group | Run the community | Consent (joined voluntarily) | Member leaves, is removed after 14 days of silence (published rule), or the community closes | Ends at removal | Remove from the group; update row 2 status |
| 7 | Webinar attendance and recordings, if any | Webinar platform `[owner to name]` | Live session; recap for members | Consent; tell attendees before recording | Recap no longer offered | Owner to set | Delete recordings and attendance exports |
| 8 | Public Threads replies | Threads (not copied) | Content research: themes only | Not collected: themes are recorded, never people (`data-handling.md`) | n/a | Not stored | n/a |
| 9 | Counts with no identifiers | `CONTENT/performance-log.md` | Measure the journey | Not personal data | n/a | No limit needed | n/a |
| 10 | Paid-service records (coaching, if it resumes) | Not collected now | Contract, payment, invoices | Contract, plus any record-keeping law (for example tax) | Set by those laws | **Reviewer to name the statutory period**, if any | Per that law |

**Never kept, so no retention period applies:** screenshots of chats, balances, deposits, income, debts, broker account details or logins (`enquiry-schema.md`).

**Retention log.** The owner records each deletion (date, row type, how many records, no identifiers). This shows the retention rule is applied in practice. Reviewer to confirm whether the Personal Data Protection Standard 2015 requires a disposal record.

**Factors for setting each period:** how long the purpose actually lasts (for example, from first message to joining the community); how long a "no reply" enquiry is worth keeping; whether the owner needs to show consent after deletion; backup cycles; any legal hold.

## 5. Proposed notice `[COMPLIANCE REVIEW REQUIRED]`

A short notice in the WhatsApp reply, linking to a full notice. Wording assumes the three questions are optional (section 6, decision 1).

**Short notice, Malay**

```
Privasi: Aku simpan nombor, nama WhatsApp dan jawapan kau (kalau kau jawab) untuk hantar PDF, info community dan susun soalan kau. Jawab soalan tu pilihan. Rekod disimpan dalam WhatsApp dan rekod peribadi aku; penyedia servis ni mungkin simpan data luar Malaysia. Aku tak jual data kau, dan tak kongsi dengan pihak lain untuk kegunaan mereka. Nak tengok, betulkan atau padam data kau, mesej aku. Nak berhenti terima mesej, type STOP. Notis penuh: [link]
```

**Short notice, English**

```
Privacy: I keep your number, WhatsApp name and your answers (if you answer) to send the PDF and community information and to organise your questions. Answering is optional. Records are kept in WhatsApp and my private records; these providers may store data outside Malaysia. I don't sell your data or share it with anyone else for their own use. To see, correct or delete your data, message me. To stop messages, reply STOP. Full notice: [link]
```

If the answers are made a condition for the community link, replace the optional sentence with: "Jawapan diperlukan untuk dapat link community. Tak jawab, kau masih dapat PDF." / "Answers are needed for the community link. Without them you still get the PDF."

**Full notice: sections** (both languages)

1. Who we are: THE MARKET DOCTRINE; data controller `[owner to supply]`; contact for privacy requests `[owner to supply]`.
2. What we collect, and from whom (from you, when you message us).
3. Why: PDF, community information, organising enquiries, fitting education to you.
4. Voluntary or required, and what happens if you don't answer.
5. Who holds it: the owner, and service providers that store or send messages (WhatsApp, Google, the webinar platform), possibly outside Malaysia. We don't sell your data or share it with anyone else for their own use.
6. How long we keep it: the retention schedule, once periods are set.
7. Your rights: access, correction, withdrawing consent, stopping messages, data portability; how to ask; how long a reply takes `[reviewer to advise]`.
8. Complaints: to the owner first; the Personal Data Protection Commissioner.
9. Version and date.

## 6. Decisions needed from the owner

1. **Questions optional or required for the community link?** Recommended: optional, as the TMD_MAGNET journey proposed. Then published posts stop saying "Jawab 3 soalan, aku bagi link" from the next batch. If required, the notice must say so (wording above).
2. **Data controller name and privacy contact.**
3. **Tools that hold data:** WhatsApp (personal or Business), the private store, the webinar platform, and whether webinars are recorded.
4. **"Aku tak jual data kau, dan tak kongsi dengan pihak lain."** Confirm it is true today and will stay true, including in any IB relationship. If data might ever go to a broker, the notice and consent must change first (and the broker gate must be open).
5. **Where the full notice lives:** a Google Doc link, a pinned community message or a future web page.
6. **Who reviews it:** a lawyer or data protection consultant familiar with the Act.
7. **Retention periods** for rows 1–7, after the reviewer's advice.

## 7. Operational points from the 2024 amendments

Reported in force on 1 June 2025 (dates from secondary sources; the Act came into force in phases on 1 January, 1 April and 1 June 2025):

| Change | What it may mean for TMD | Confidence |
|---|---|---|
| Data breach notification | If the phone, WhatsApp, Google account or private sheet is compromised, the Commissioner must be notified as soon as practicable. Affected people may also need to be told. Several firms cite 72 hours from the Commissioner's guideline; one source could not confirm that figure. Write a one-page breach plan. | Medium. Reviewer to confirm the timing |
| Data Protection Officer | Required above thresholds set in a guideline. One summary cites over 20,000 data subjects, over 10,000 for sensitive data, or regular and systematic monitoring. TMD is likely below them. | Medium. Reviewer to confirm |
| Data portability | People can ask for their data to be sent to another provider, where technically feasible | Medium-high |
| Processors bound by the Security Principle | Applies to anyone who processes data for the owner, such as an assistant or a tool | Medium-high |
| Higher penalties | Penalties were raised. The amount was not confirmed in this review. | Confirmed raised; figure not verified |

## Sources (secondary; read 18 Nov 2026)

- DataGuidance — Personal Data Protection (Amendment) Act 2024: key changes. https://www.dataguidance.com/opinion/malaysia-personal-data-protection-amendment-act
- Baker McKenzie — Malaysia: Personal Data Protection (Amendment) Act 2024 to come into force. https://www.bakermckenzie.com/-/media/files/insight/publications/alerts/08/malaysia-public-consultation-on-the-personal-data-protection-regulations/malaysia-personal-data-protection-amendment-act-2024-to-come-into-force--ba.pdf
- DLA Piper — Data protection laws of the world: Malaysia. https://www.dlapiperdataprotection.com/?t=law&c=MY
- BlackTree — Malaysia's privacy reform puts DPOs and breach notices on the clock (4 Jun 2025). https://blacktree.nl/2025/06/04/malaysias-privacy-reform-puts-dpos-and-breach-notices-on-the-clock/
- Ridza Law — Malaysia's Personal Data Protection (Amendment) Act 2024. https://www.ridzalaw.com.my/post/malaysia-s-personal-data-protection-amendment-act-2024
- Rahmat Lim & Partners — Amendment Bill 2024 passed by Parliament. https://www.rahmatlim.com/perspectives/articles/28434/mykh-personal-data-protection-amendment-bill-2024-passed-by-parliament
- Edwin Lee & Partners — 20 FAQs on the PDPA 2010 (updated for the 2024 amendments). https://lpplaw.my/insights/e-articles/faq-pdpa-2010/
- CecoLaw — PDPA Malaysia: 2024 amendments. https://www.cecolaw.com/data-privacy-law-in-malaysia/

Primary sources for the reviewer: the Act as amended, the Personal Data Protection Standard 2015, and the Commissioner's guidelines on breach notification, DPOs and cross-border transfers (Personal Data Protection Department).

## Checks

Shared checklist: PASS — no personal data; facts and assumptions labelled; secondary-source points flagged with confidence.
Agent checks: PASS — notice at first contact, marked `[COMPLIANCE REVIEW REQUIRED]`; opt-out and its effect stated; no coaching, broker, account or deposit step; questions limited to the schema; no retention period invented.
Needs the owner: the seven decisions in section 6, and a qualified reviewer.
