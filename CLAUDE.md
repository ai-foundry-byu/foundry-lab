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

- **Positioning**: an AI-native product studio and consultancy. We ship production software, we
  do not deliver reports. Source of truth is the one-pager, `~/Desktop/AI-Foundry.pdf`
- **Three offerings**: full-stack applications; AI integration and orchestration; AI enablement
  and training
- **Three phases**: 01 Audit and discovery, 02 Build, 03 Transfer
- **Pricing (set 2026-08-01)**: $22,000 fixed fee for an 8-month engagement. Derived from $35
  per student-hour: 2 builders x 10 hrs/week x 32 weeks = 640 hours = $22,400, rounded to
  $22,000. Publish the $22,000 and the team shape; the hourly is internal. Discovery-only is
  scoped separately and priced smaller
- **Team**: 15 MBAs and roughly 15 undergraduate builders in mixed teams. Per-engagement roles
  are client lead, builders, QC lead
- **Intake**: rolling. No application deadline, no fixed milestone calendar. Phase dates are set
  per engagement at kick-off. Do not reintroduce fixed dates into partner-facing pages
- **Scott's title**: Faculty Advisor
- **Contact**: aifoundry.byu.edu, aifoundry@byu.edu
- **Key student deliverable**: weekly client update, sent Saturday by 11:59 PM by the client lead

## Open Decisions

See `DECISIONS.md`. Several program parameters are proposed defaults, not confirmed policy.
Do not present them to clients as final until that file is cleared.

## House Style

- No em dashes anywhere in this repository
- Plain, factual prose. Scott adds the flourishes
