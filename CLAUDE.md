# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Quarto book for the **BYU AI Foundry Lab**, a year-long sponsored-project studio in the BYU
Marriott School of Business. Cross-listed as **MBA 693R** (section 011, Special Topics in
Management) and **STRAT 490R** (section 001, Topics in Strategic Management), Fridays
8:00 to 11:50 AM in 2140 TNRB, 3.0 credits per semester.

The site serves three audiences: students on Foundry teams, sponsoring client partners, and
prospective sponsors reading the RFP.

Mirrors the structure of `byu-strategy/apm-lab`, with cross-listing presentation borrowed from
`byu-strategy/product-management`.

## Build Commands

- **Preview during development**: `quarto preview`
- **Check installation**: `quarto --version`

**Never render locally.** The site auto-renders via GitHub Actions on push to main. See
`.github/workflows/publish.yml`. Output goes to `docs/`.

## Content Structure

```
index.qmd                       # Program overview, cross-listing, key dates

students/
  01-syllabus.qmd               # Grading, policies, confidentiality, AI use, BYU boilerplate
  02-getting-started.qmd        # Onboarding, team roles, first two weeks
  03-weekly-updates.qmd         # Weekly client email format and examples
  04-build-standards.qmd        # Quality bar, repo standards, decision log, QC gate

partners/
  01-program-overview.qmd       # Structure, milestones, what we do and do not do
  02-working-with-the-team.qmd  # Cadence, scoping, scope changes
  03-evaluation.qmd             # Mid-year and end-of-year feedback
  04-faq.qmd                    # Cost, IP, confidentiality, fit, hiring
  05-rfp.qmd                    # Partner-sourcing page, mirrors the engineering capstone RFPs
```

## Cross-Listing Pattern

Two places carry the course numbers, following `byu-strategy/product-management`:

1. `_header.html` injects `.sidebar-course-numbers` under the sidebar title
2. `index.qmd` and `students/01-syllabus.qmd` open with a `.course-numbers-page` div, followed
   by a "Course Numbers" section with the section-and-title table

Styles for both classes live at the bottom of `styles.css`.

## Program Context

- **Duration**: 8 months, September 2, 2026 to April 14, 2027
- **Teams**: 4 to 6 students, roles are client lead, builders, QC lead
- **Sponsorship**: $22,000 per project, sponsor retains all IP
- **Milestones**: M1 framework (Oct 16), M2 prototype (Dec 11), M3 validated model (Feb 19), M4 delivery (Apr 9)
- **Key student deliverable**: weekly client update, sent Saturday by 11:59 PM by the client lead

## Open Decisions

See `DECISIONS.md`. Several program parameters are proposed defaults, not confirmed policy.
Do not present them to clients as final until that file is cleared.

## House Style

- No em dashes anywhere in this repository
- Plain, factual prose. Scott adds the flourishes
