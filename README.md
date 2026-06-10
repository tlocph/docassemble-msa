# docassemble-msa

MSA w/o Children — a [docassemble](https://docassemble.org) extension package
that generates a **California Marital Settlement Agreement** (MSA) for a
dissolution of marriage **without minor children**.

## What it does

The guided interview collects, in a handful of grouped screens:

1. **Parties** — the spouses' names, which spouse is the Petitioner, and the
   Petitioner's contact information (for the In Pro Per heading)
2. **Case information** — county, case number, dates of marriage, separation,
   and the agreement
3. **Property** — each spouse's separate property and any community property
   being transferred (blank entries render as "No Property")
4. **Debts** — debts each spouse will assume (blank entries render as "Each
   party will be responsible for their own debt.")
5. **Spousal support** — a mutual waiver, or monthly payment terms (payor,
   amount, start date, and termination conditions)

It then assembles a pleading-formatted MSA as PDF or DOCX, including the
court caption, recitals, warranties, boilerplate clauses, signature blocks,
and the judge's order line.

## Files

- `docassemble/msa/data/questions/msa.yml` — the interview
- `docassemble/msa/data/templates/Marital_Settlement_Agreement.docx` — the
  Jinja2 DOCX template

## Installation

Install through the docassemble **Package Management** screen using this
repository's URL, or test it via the Playground.

Run the interview at:

```
/interview?i=docassemble.msa:data/questions/msa.yml
```

## Disclaimer

This package does not provide legal advice. Have an attorney review any
generated agreement before signing or filing it.
