# Client Intake Form

The questions a prospective partner answers before the scoping call. Every question exists
because its answer changes staffing, scoping, or pricing. If a question does not move one of
those three, it is not on the form.

Built to be published as a Google Form on the `aifoundry.byu@gmail.com` account, linked from
the RFP page in place of the current bare `mailto:`.

**Signal column** shows what the answer feeds. Archetype codes and risk tiers are defined in
`staffing-model.md`.

---

## Section 1. Who you are

| # | Question | Type | Signal |
|---|---|---|---|
| 1 | Company name | Short text | Record |
| 2 | Website | Short text | Record |
| 3 | Your name, title, email, phone | Short text x4 | Record |
| 4 | Are you the person who can approve scope and budget? If not, who is? | Short text | Sponsor authority. A referred project with no named approver stalls |
| 5 | How did you hear about us? | Choice: CapSource, BYU referral, faculty, search, other | Channel attribution |

## Section 2. The problem

| # | Question | Type | Signal |
|---|---|---|---|
| 6 | In two or three sentences, what problem do you want solved? | Paragraph | Everything |
| 7 | What happens today, without this? Who does the work and how? | Paragraph | Baseline. Reveals whether there is a real workflow to replace |
| 8 | How will you know it worked? Name the number that moves. | Paragraph | Whether the client has a success definition. If they cannot answer this, sell discovery |
| 9 | Is this a problem you have already tried to solve? What happened? | Paragraph | Prior failure is the best predictor of hidden complexity |

## Section 3. What you want built

| # | Question | Type | Signal |
|---|---|---|---|
| 10 | Which best describes it? Select all that apply: net-new web or mobile app / AI agent or copilot over your data / automation of an existing workflow / analytics, forecasting, or a decision model / replacing a tool you currently pay for / not sure, we want the audit | Multi-select | **Primary and secondary archetype** |
| 11 | Who uses it, and roughly how many of them? Internal staff, your customers, the public? | Paragraph | Archetype E, risk tier, auth and roles hours |
| 12 | Is there an existing product or vendor this replaces or sits next to? Name it. | Short text | Sizing. Replacement implies feature parity expectations and data migration |
| 13 | If we shipped one thing in eight months, what is the single most important piece? | Paragraph | The scope anchor. Quoted back verbatim in the phase 02 scope |
| 14 | What is explicitly out of scope, as far as you are concerned? | Paragraph | Written before the relationship exists, which is when honest answers happen |

## Section 4. Technical environment

| # | Question | Type | Signal |
|---|---|---|---|
| 15 | Do you have engineers on staff? How many, and will any work with us? | Short text | Transfer phase design. No engineers means transfer is training, not handoff |
| 16 | What is your current stack and hosting, if any? | Paragraph | Archetype match. Constrains builder selection |
| 17 | Who will own the code repository, you or us during the build? | Choice | IP and access logistics |
| 18 | List every system this must connect to. One per line. | Paragraph | **Integration count, hour estimate, risk tier** |
| 19 | Can you provision accounts and API access for a student team within two weeks of kickoff? | Choice: yes / no / unsure | Single most common cause of a stalled build |

## Section 5. Data

| # | Question | Type | Signal |
|---|---|---|---|
| 20 | What data will the team need to see? | Paragraph | Risk tier |
| 21 | Does any of it include: personal information about identifiable individuals / health information / education records / records about minors / payment or financial account data / none of these | Multi-select | **Risk tier. Restricted if any of the first four** |
| 22 | Do you have data available today, or does it need to be collected or cleaned first? | Choice | Archetype C hours. Unclean data can consume a phase |
| 23 | Do you require your own NDA, or is our standard mutual NDA acceptable? | Choice | Legal path and timing |

## Section 6. If AI makes or influences a decision

Only shown when question 10 includes an AI option.

| # | Question | Type | Signal |
|---|---|---|---|
| 24 | Will the system's output influence a decision about a person? Hiring, admission, credit, credentialing, care, discipline? | Choice: yes / no | **Escalates to Restricted. Triggers the adverse impact conversation before the proposal** |
| 25 | If yes, who reviews the output before the decision is made? | Paragraph | Human-in-the-loop design. Required, not optional |
| 26 | What does a wrong answer cost you? | Paragraph | Accuracy target, eval design, archetype B hours |
| 27 | Do you have labeled examples of good and bad outcomes we can learn from? | Choice plus paragraph | Whether scoring can be validated at all inside 8 months |

## Section 7. Design

| # | Question | Type | Signal |
|---|---|---|---|
| 28 | Do you have brand assets, a design system, or existing UI we should match? | Choice plus upload | **Archetype E. Net-new design adds 60 to 100 hours** |
| 29 | Is design quality a priority for this, or is it an internal tool where function is enough? | Choice | Whether the Design Lead is named to the pod |

## Section 8. Timing, budget, commitment

| # | Question | Type | Signal |
|---|---|---|---|
| 30 | When would you want to start? | Choice: as soon as possible / next semester / flexible | Queue position against the 6-pod cap |
| 31 | Is there a hard external deadline? What drives it? | Paragraph | Immediate disqualifier if it does not fit the phase structure |
| 32 | Our standard engagement is $22,000 fixed for 8 months, covering discovery, build, and transfer. Is that workable? | Choice: yes / need to discuss / we want discovery only first | Qualification |
| 33 | Who is the single weekly point of contact, and can they hold a standing 30 to 45 minute call? | Short text plus choice | Hard requirement. No named POC, no engagement |
| 34 | Can you turn around decisions the team raises within one week? | Choice | Sets the decision SLA in the scope document |
| 35 | May we name you publicly as a partner and use the work as a case study? | Choice: yes / after launch / no | Marketing |

## Section 9. Anything else

| # | Question | Type |
|---|---|---|
| 36 | What have we not asked that we should have? | Paragraph |
| 37 | Attach anything useful: specs, screenshots, an RFP you already wrote | File upload |

---

## Screening rubric

Filled by the Director of External Deals within two business days of submission.

### Fit, 0 to 2 each

| Criterion | 0 | 1 | 2 |
|---|---|---|---|
| Real problem, articulated | Vague | Named but no baseline | Baseline and success metric both given |
| Something ships | Research only | Prototype acceptable | Production software wanted |
| Sponsor commitment | No named POC | Named, unsure on cadence | Named, weekly call confirmed, decision SLA accepted |
| Access provisionable | No or unsure | Probably | Yes, within two weeks |
| Fits 640 hours | Estimate over 1000 | 640 to 1000, needs narrowing | Under 640 |
| Bench can staff it | No level-3 in the primary archetype | Level 3 exists, no two-deep | Level 3 plus two-deep |

**11 to 12** proceed to scoping call. **7 to 10** scoping call, expect to sell discovery only.
**Below 7** decline, or offer discovery with an explicit statement that the build phase is not
promised.

Any zero on "bench can staff it" or "sponsor commitment" is an automatic decline for the build
phase regardless of total.

### Output

The screen produces a one-paragraph staffing brief seed: primary archetype, secondary
archetype, risk tier, rough hour estimate, and the single largest delivery risk. That is what
goes into the scoping call and, after it, into the auction posting.

---

## Worked example: Indigo Institute, received 2026-08-10

Vocational training and staffing company for dental assistants, Provo Kiln. Kim Moore, CEO.
Two projects requested in one email.

**First conclusion: this is two engagements, not one.** Section 4 of the staffing model says
one pod ships one product surface. An AI video interviewing system and a full LMS are two
products with almost no shared surface. Quote them separately at $22,000 each, or sequence
them. They may share an Engagement Lead, which is worth doing since the domain context is the
same company.

### Project 1, video interviewing and candidate screening

| | |
|---|---|
| Primary archetype | B, AI and agents |
| Secondary | A, full-stack application |
| Risk tier | **Restricted** |
| Rough estimate | Video capture and storage 100 to 150, scoring layer with evals 100 to 160, auth and admin 80 to 120, ATS integration 40 to 80. Roughly 320 to 510, plus discovery. Fits 640 if scope holds |
| Named incumbent | HeyMilo AI. Feature-parity expectations are live from day one |

Restricted because the output scores candidates and influences a hiring and admissions
decision. Question 24 is exactly this case. Before a proposal goes out, three things get
settled in writing: Indigo owns the hiring decision, a human reviews every score, and the
Foundry does not validate the instrument for adverse impact. Video interview recordings of
applicants are also personal data at volume, so question 21 lands and the NDA precedes any
data transfer.

Staffing note: needs a builder rated 3 in B, plus the two-deep name. This is the harder of the
two to staff.

### Project 2, next-generation LMS

| | |
|---|---|
| Primary archetype | A, full-stack application |
| Secondary | E, product design |
| Risk tier | Elevated, possibly Restricted |
| Rough estimate | Well over 640 as described |

The request as written is progress tracking, gamification, instructor and admin dashboards, AI
learning support, personalized feedback, and adaptive testing. Adaptive assessment alone is a
capstone. This does not fit one engagement and should not be quoted as though it does.

The move is a discovery-only engagement that cuts it to one shippable surface, most likely
student progress tracking plus the instructor dashboard, with AI feedback as phase 2 of a
second year. Question 13 is the one that forces that conversation, which is why it is on the
form.

Elevated to Restricted depends on whether student records are education records under FERPA.
Indigo is a private vocational provider, so probably not FERPA, but confirm rather than assume,
and ask whether any students are minors.

### What to send Indigo

The intake form, once. Both projects, one submission each. Then a single 45-minute scoping call
covering both, and a proposal that prices them separately and is honest that the LMS as
described is larger than one engagement.
