# STATUS — Healthcare Administration Freebies Kit

## What was built

A freebies kit (Markdown + printable HTML) for healthcare administration, created and published by **Asdale Dynamics, LLC** (Indiana, formed October 2026). Four fillable, printable, large-print-friendly forms, each as a standalone HTML file plus an editable Markdown version:

| HTML file | Markdown file | Purpose |
|-----------|---------------|---------|
| `forms-completeness-checklist.html` | `forms-completeness-checklist.md` | Verify admission/encounter paperwork is complete before it leaves the unit (ID/demographics, consents, insurance/billing, clinical documentation, discharge/follow-up) |
| `deadline-calendar.html` | `deadline-calendar.md` | Monthly deadline calendar with a 12-row task tracker and a 31-day calendar grid |
| `meeting-prep-sheet.html` | `meeting-prep-sheet.md` | Prepare for and document care-team meetings (purpose, attendees, agenda, pre-work, decisions, action items, follow-up) |
| `policy-draft-template.html` | `policy-draft-template.md` | Draft department policies section by section (purpose, scope, statement, definitions, procedure, responsibilities, compliance, references, revision history, approval) |

Also included:
- `LICENSE` — MIT License, copyright line exactly `Copyright (c) 2026 Asdale Dynamics, LLC`
- `README.md` — usage, accessibility, education-only disclaimer, credit to Asdale Dynamics, LLC

## How to run

No build step, no account, no install. All files are local-first and run entirely in the browser:

1. Open any `.html` file in Chrome, Edge, Firefox, or Safari.
2. Fill in fields on screen (inputs, checkboxes, text areas) or print and complete by hand.
3. Print with your browser's Print command (Ctrl+P / Cmd+P), or click the "Print this form" button on screen.
4. Pages are sized for US Letter with print-optimized CSS (header/footer buttons hidden, borders sharpened, backgrounds removed).

The Markdown `.md` files are for editing, copying, and accessibility; they render in any Markdown viewer.

## Verification results

- All four HTML files parse without structural errors (validated with Python's `html.parser`; reported "mismatches" are false positives from void elements like `<input>` and `<meta>`, which require no closing tag).
- `LICENSE` copyright line verified: `Copyright (c) 2026 Asdale Dynamics, LLC` (exact match).
- `README.md` credits Asdale Dynamics, LLC and links to dylanasdale.github.io.
- Git initialized and committed as `a5aae03` with plain message "Add healthcare administration freebies kit" (10 files, 943 insertions). No Co-authored-by trailers, no push, no remote, no `.github/workflows`.
- No secrets, API keys, or personal data in any file.

## Known gaps

- No automated test suite or linter is configured (intentionally; this is a static HTML/Markdown kit with no build pipeline). Verification was manual parse + visual review.
- Calendar grid is pre-numbered 1–31; the user must shade/circle the correct starting weekday for the target month manually. No JavaScript date generation was added to keep files dependency-free and printable without scripting.
- Print rendering depends on the browser's print engine; page breaks may vary slightly by browser. Tested conceptually via print media CSS; not across every browser/OS combination.
- These are education-only administrative aids, not medical or legal advice; each form carries its own disclaimer.
