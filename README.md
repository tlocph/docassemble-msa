# docassemble-msa

A [docassemble](https://docassemble.org) extension package that generates a
California **Consent for Minor Child(ren) to Travel** — the letter the
non-traveling parent signs so the other parent (or legal guardian) can
travel with the children.

## What it does

The guided interview collects, in a handful of grouped screens:

1. **Consenting parent** — name, relationship, address, phone, and email of
   the parent staying home
2. **Children** — any number of children, each with name, date of birth,
   place of birth, and optional passport details
3. **Traveling parent** — name, relationship, address, phone, and optional
   passport/ID number
4. **Travel details** — destination(s), departure and return dates, mode of
   travel, accommodations, purpose, and identification of any existing
   custody order
5. **Signature** — date and city of execution

It then assembles the consent letter as PDF or DOCX, including the
day-to-day decision and emergency medical authorizations, the penalty of
perjury declaration, and a California notary acknowledgment block
(Civil Code § 1189).

## Files

- `docassemble/msa/data/questions/minor_travel_consent.yml` — the interview
- `docassemble/msa/data/templates/Minor_Travel_Consent.docx` — the Jinja2
  DOCX template

## Installation

Install through the docassemble **Package Management** screen using this
repository's URL, or test it via the Playground.

Run the interview at:

```
/interview?i=docassemble.msa:data/questions/minor_travel_consent.yml
```

## Disclaimer

This package does not provide legal advice. Notarization is strongly
recommended for international travel and may be required by airlines or
foreign authorities.
