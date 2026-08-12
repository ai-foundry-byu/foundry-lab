# AI Foundry Staffing Model

Internal. Not published to the site. Sets how people get assigned to client engagements,
what the bench can absorb, and what has to be true before a pod is declared staffed.

Consistent with the published RFP: 2 dedicated builders, plus a QC lead and faculty
oversight, 20 team-hours per week, 640 hours over 8 months, $22,000 fixed.

## 1. The unit of delivery is a pod

One engagement, one pod. A pod is the smallest group that can find the problem, build the
thing, and hand it over without a handoff inside the team.

| Role | Who | Load | Shared? |
|---|---|---|---|
| Engagement Lead | MBA | 4 hrs/wk | Up to 2 engagements |
| Builder A (primary) | Undergrad or technical MBA | 10 hrs/wk | Never. One engagement only |
| Builder B | Undergrad or technical MBA | 10 hrs/wk | Never. One engagement only |
| QC Lead | Product Eval and QC function (Tulga Ganbat) | 2 hrs/wk per pod | Up to 4 pods |
| Design Lead | UX/UI function (John Passey) | 2 hrs/wk, on demand | Across all pods |
| Faculty Advisor | Scott Murff | Oversight | All pods |

Only the two builders are billed capacity. The lead, QC, and design hours are overhead the
fixed fee absorbs, which is why builder hours are the thing that must never be double-booked.

**Engagement Lead** owns the client relationship: the weekly call, scope, the decision log,
the weekly update, and escalation. Owns the answer to "is this still inside 640 hours."

**Builders** write the code and ship it. Builder A is accountable for the architecture.

**QC Lead** is a gate, not a reviewer of convenience. Nothing reaches the client without
passing it. Applies the build standards, reviews architecture at kickoff and at each phase
boundary, and signs the transfer.

**Design Lead** is pulled in for anything with a real end-user surface. Sets the design
direction in week 1 and 2, then reviews.

## 2. Skill archetypes

Every project is classified into a primary and a secondary archetype at intake. Every
builder on the bench carries a 0 to 3 rating in each. This is the matching key.

| Code | Archetype | What it looks like |
|---|---|---|
| A | Full-stack application | Net-new web or mobile app, auth, database, deploy |
| B | AI and agents | LLM pipelines, scoring, evals, RAG, agent orchestration |
| C | Data and modeling | Forecasting, optimization, analytics, decision frameworks |
| D | Integration and automation | APIs, webhooks, document processing, workflow glue |
| E | Product design | UX/UI-heavy, design system, net-new interface |
| F | Domain and strategy | Regulated industry, market analysis, business rules |

Ratings: 0 none, 1 coursework only, 2 has shipped it once, 3 can lead it and teach it.

**Matching rule.** A pod is validly staffed when:

1. At least one builder is rated 3 in the project's primary archetype.
2. Combined, the two builders are rated 2 or better in the secondary archetype.
3. No builder is on any other active engagement.
4. A second bench member outside the pod is rated 3 in the primary archetype. This is the
   two-deep rule and it exists so one student dropping the course does not kill an engagement.

If rule 1 or rule 4 fails, do not sign the build phase. Sell discovery only, or decline.

## 3. Capacity

15 undergraduate builders, two per pod, is 7 pods. Hold one back.

| | |
|---|---|
| Builder bench | ~15 undergraduate builders, plus technical MBAs |
| Maximum concurrent engagements | **6** |
| Float pod | 1, held unstaffed for recovery, overrun, and a late high-value client |
| MBA engagement leads needed at full load | 3 to 6 of 15 |
| QC leads needed at full load | 2 (4 pods each) |

The binding constraint is builder hours, not MBAs. The MBA bench is oversupplied relative to
the builder bench, so the growth lever is undergraduate recruiting, not deal flow.

When all 6 pods are staffed, new engagements queue. The RFP already says this. Do not solve
a full bench by putting a builder on two pods.

## 4. One pod ships one product surface

640 hours is enough for one focused product. It is not enough for two.

When a client brings more than one project, each becomes its own engagement, its own fee,
and its own pod. They may share an Engagement Lead, which is the only sensible economy,
because the client relationship and the domain context genuinely transfer.

Sizing check at intake, in builder hours:

| Signal | Hours it tends to add |
|---|---|
| Auth, roles, and an admin surface | 80 to 120 |
| Each third-party integration | 40 to 80 |
| Video capture, storage, and processing | 100 to 150 |
| An AI scoring or evaluation layer with evals | 100 to 160 |
| Net-new design system, no client brand assets | 60 to 100 |
| Compliance review (PHI, FERPA, minors) | 40 to 80 |
| Data migration from an incumbent system | 60 to 120 |

If the estimate clears 640, the answer is not a bigger team. The answer is a narrower phase
02 scope, or a second engagement, priced separately.

## 5. Risk tiers, and what they add to staffing

| Tier | Triggers | Staffing consequence |
|---|---|---|
| Standard | Internal tool, no regulated data, 0 to 2 integrations | Base pod |
| Elevated | Customer-facing, PII, 3 or more integrations, replaces a paid incumbent | QC lead at 4 hrs/wk, Design Lead named, phase 02 scope reviewed by faculty before signing |
| Restricted | PHI, FERPA, records on minors, payments, anything a regulator inspects | All of the above, plus a named data-handling owner in the pod, client NDA before any data moves, and an explicit written carve-out that the Foundry does not make clinical, credentialing, or compliance determinations |

Hiring and candidate-screening tools sit at Elevated by default and go to Restricted the
moment a scoring output influences an employment or admissions decision. That is adverse
impact territory. The team can build the tool. The client owns the decision and the
validation, in writing.

## 6. Intake to kickoff

| Step | Owner | Clock |
|---|---|---|
| 1. Intake form submitted | Client | Day 0 |
| 2. Fit and complexity screen | Director, External Deals | 2 business days |
| 3. 45-minute scoping call | Scott plus proposed Engagement Lead | Week 1 |
| 4. Staffing brief written | Engagement Lead | 3 days after call |
| 5. Pod named and confirmed against the matching rule | Scott plus QC function | Same week |
| 6. Discovery scoped and signed | Scott | Week 2 |
| 7. Kickoff, architecture review | Pod plus QC lead | Week 3 |

The staffing brief is one page: primary and secondary archetype, risk tier, hour estimate
against the table in section 4, proposed pod, the two-deep name, and the single biggest
delivery risk.

Nobody is told they are staffed on an engagement before step 6. Signed scope first.

## 7. Discovery-only staffing

A discovery-only engagement is not a pod. It is the Engagement Lead plus one builder, 4 to 6
weeks, and it exists to answer the sizing question in section 4 with evidence instead of a
guess. The builder who runs discovery gets first claim on Builder A if the build phase signs,
because the context is worth more than the scheduling convenience.

## 8. Rules that do not bend

1. A builder is on exactly one engagement.
2. Every pod has a named Engagement Lead and a named QC Lead before kickoff.
3. No pod is staffed against unsigned scope.
4. Two-deep on the primary archetype, or no build phase.
5. Maximum 6 concurrent engagements, seventh pod held as float.
6. One pod ships one product surface. A second product is a second engagement.
7. Client data stays in the approved repo and approved tools. Deleted at transfer.

## 9. Builder preference: the points market

Fit decides who is eligible. Points decide who among the eligible gets the seat.

### The currency

| | |
|---|---|
| Accrual | 100 points per month, every enrolled builder |
| Cap | 300 points. Accrual stops at the cap |
| While staffed | Points keep accruing, still capped at 300 |
| On winning a seat | Balance resets to zero |
| Rollover between semesters | Yes, subject to the cap |
| Other uses | None. Points buy seats, nothing else |

The cap and the reset are what stop the market from being decided by who has been idle
longest. A builder who has been on the bench since September should have an edge over one
placed last month, but not an insurmountable one.

### The auction

1. A new engagement signs. Staffing publishes the project one-pager, the primary and
   secondary archetype, the risk tier, and the estimated hours.
2. **The fit gate runs first.** Staffing publishes the eligible roster for that project:
   every bench builder who clears the archetype rating for the seat being auctioned and is
   free of any other engagement. Ineligible students cannot bid and lose nothing.
3. **Builder A is appointed, not auctioned.** Staffing names the builder rated 3 in the
   primary archetype, and confirms the two-deep name on the bench.
4. **Builder B is auctioned.** Sealed bids from the eligible roster, 72-hour window, one bid
   each, no revisions.
5. **Second price.** Highest bid wins and pays the second-highest bid plus one point. Ties
   break toward the builder with fewer completed engagements, then by coin flip.
6. Losing bidders pay nothing and keep their balance.
7. Bids and clearing prices are published after each auction. Students should be able to see
   what projects have cleared at historically.

Second price is deliberate. It makes bidding your true level of interest the correct
strategy, so the number carries information rather than measuring who is best at guessing
what everyone else will do.

### Guardrails

- **Fit is never overridden by points.** A high bid from an ineligible builder is not a bid.
- **Nobody goes unstaffed for a semester.** Any builder with zero engagements by the midpoint
  of the term gets a directed placement into the next opening, outside the auction. The
  market allocates enthusiasm, it does not decide who gets to participate.
- **The client never sees this.** Internally it is a preference market. Externally the pod
  was staffed on fit, which is true, because fit gated it.
- **Faculty veto exists and gets used sparingly.** Restricted-tier engagements can be closed
  to the auction entirely and staffed by appointment.
