# Prospects

**No prospect or enquiry records are stored in this repository.**

## Why

- Git history is permanent: a record committed once stays in history even after the file is deleted.
- The repository lives on GitHub, outside the owner's direct control.
- Enquiry records are personal data. Malaysia's Personal Data Protection Act 2010 is likely to apply (flag, not legal advice).

## Where records go

A private store the owner controls, such as a Google Sheet in the owner's account with access limited to the owner. Records are entered by a person, not by an automated process.

## What lives here

- This README.
- Nothing else. The record structure is defined in `AGENTS/TMD_PROSPECT_INTELLIGENCE/enquiry-schema.md`.

Aggregate counts with no identifiers (by week, source, keyword, segment) may be recorded in `CONTENT/performance-log.md`.

## Safety net

`.gitignore` excludes `PROSPECTS/private/` so an accidental file there is not committed. It is not a storage location: anything saved there exists only on the machine where it was saved, and a cloud session's machine is deleted when the session ends.
