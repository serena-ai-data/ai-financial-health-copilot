# Technical Product Ownership — Delivery Plan

This document extends the public prototype into a product-owner view of how the MVP could be scoped, handed to engineering, launched and iterated. It is a portfolio design artefact, not a claim that these releases have already shipped.

## 1. Product boundary and system flow

The product deliberately separates financial facts and calculations from AI-generated interpretation.

`User / financial source -> validation & review -> deterministic rules engine -> financial state -> AI explanation layer -> user interface`

### Deterministic source of truth

The deterministic layer owns:

- confirmed balances and user-entered financial facts;
- calculation inputs and formulas;
- financial-health score classification;
- transaction state;
- rule-based eligibility or threshold logic;
- audit-friendly calculation outputs.

### AI-assisted layer

The AI layer may:

- explain verified results in plain language;
- summarise complex financial information;
- surface missing context and uncertainty;
- answer grounded questions about the user's results;
- help prioritise what the user should review next.

The AI layer must not silently alter verified facts, balances, score calculations or transaction states.

## 2. Prioritised MVP backlog

| Priority | Product item | User value | Why now |
| --- | --- | --- | --- |
| P0 | Consent and AI-boundary disclosure | Understand how sensitive data and AI are used | Required before collecting financial data |
| P0 | Structured financial input | Create a usable financial picture | Core data needed for the first insight |
| P0 | Review and correction | Prevent incorrect inputs from driving outputs | Trust and data-quality control |
| P0 | Deterministic financial-health analysis | Produce reproducible results | Source of truth for consequential calculations |
| P1 | Explainability view | Understand why a score or action appears | Builds trust and supports correction |
| P1 | Prioritised next-best action | Know what deserves attention first | Converts information into user value |
| P2 | AI Copilot | Ask grounded follow-up questions | Adds interpretation after the core product works |
| P2 | Connected financial data | Reduce manual input and increase continuity | Valuable after the product hypothesis is validated |

## 3. Example user story and acceptance criteria

### User story: Review and verify financial information

**As a user, I want to review the financial information that will influence my result so that incorrect or uncertain data does not silently affect the recommendation.**

### Acceptance criteria

1. The user can see every material input before analysis begins.
2. The user can edit manually entered information before confirming the analysis.
3. Any future AI-extracted field should display its source and confidence or uncertainty state where available.
4. Unconfirmed or missing information is not silently converted into a verified fact.
5. The analysis does not run until required fields are present and valid.
6. If the user changes an input, the next calculation uses the corrected value.
7. Material assumptions and demo limitations remain visible to the user.

### Edge cases to test

- income or essential expenses missing;
- negative or invalid numeric input;
- conflicting information from two sources;
- debt balance present but interest status unknown;
- incomplete protection information;
- a user asks the AI to infer an unsupported fact.

## 4. Release roadmap

### MVP — Financial understanding

- manual or synthetic input;
- consent and review;
- deterministic analysis;
- financial-health dashboard;
- explainability;
- prioritised next-best action;
- bounded Copilot interaction.

**Goal:** validate whether users can reach a useful first insight quickly and understand why it was produced.

### V2 — Connected financial context

- bank / wallet / insurance data connectors where legally and technically feasible;
- source-level traceability;
- recurring refresh;
- stronger exception and data-quality handling.

**Goal:** reduce manual input and improve continuity without weakening reviewability.

### V3 — Personalised financial actions

- goal planning;
- context-aware nudges;
- deeper protection and liquidity analysis;
- product discovery or hand-off where appropriate;
- experimentation framework for action ranking.

**Goal:** move from understanding to useful, measurable action while preserving user control.

### V4 — Governed execution

- human-confirmed transaction or product hand-off;
- suitability and eligibility controls where required;
- stronger audit trail and approval logic;
- explicit limits on autonomous AI execution.

**Goal:** support higher-value financial actions only when operational, compliance and technical controls are mature enough.

## 5. Key product trade-offs

| Trade-off | Decision for this MVP | Reasoning |
| --- | --- | --- |
| Real financial integrations vs manual input | Start with manual / synthetic input | Validate the user problem before investing in integrations |
| LLM-generated score vs deterministic score | Deterministic score | Reproducibility and auditability matter more than novelty |
| More features vs time to first insight | Narrow first workflow | Reduce cognitive load and test the core value proposition |
| Autonomous action vs human confirmation | Human remains in control | Financial actions can be consequential and require stronger safeguards |
| Hiding uncertainty vs showing incomplete context | Show uncertainty | Prevent false precision and unsupported recommendations |
| Perfect data vs useful decision | Allow bounded progress with visible limitations | The product should support decisions without pretending uncertainty does not exist |

## 6. Launch and post-launch measurement plan

These are proposed metrics for future testing. They are not claimed as measured results.

### Adoption and journey

- financial-health report completion rate;
- Time to First Insight;
- step-level drop-off rate;
- repeat usage / return rate;
- feature adoption for explainability and next-best actions.

### Data quality and trust

- input correction rate;
- percentage of material outputs with inspectable reasoning;
- source-attribution accuracy for future extracted fields;
- unresolved uncertainty rate;
- user-reported incorrect-result rate.

### AI quality and safety

- unsupported-claim rate;
- numerical-consistency rate;
- unsafe-recommendation rate;
- appropriate boundary / refusal rate;
- percentage of answers grounded in verified product state.

### Product value

- percentage of completed reports with at least one reviewed action;
- action engagement rate;
- user-reported clarity / confidence after completing the flow;
- customer-support or manual-review escalation rate in a production version.

## 7. Post-launch operating loop

`Production signal -> triage -> user / business impact -> root cause -> backlog priority -> release -> measurement -> iteration`

A product launch is not considered finished at release. Production issues, user feedback, operational friction, compliance concerns and metric movement should all feed back into backlog decisions.

### Example decision rules

- A safety or material financial-state defect overrides normal roadmap priority.
- A high-frequency journey failure is prioritised before low-usage feature expansion.
- A feature with weak adoption is investigated before adding complexity around it.
- AI behaviour that changes verified numbers or overstates certainty is treated as a release-blocking defect.

## 8. What this artefact is designed to demonstrate

This product case intentionally goes beyond concept slides. It demonstrates:

- user-problem framing;
- MVP scope and explicit out-of-scope decisions;
- functional requirements;
- backlog prioritisation;
- acceptance criteria and edge cases;
- engineering-facing system boundaries;
- product trade-offs;
- launch planning;
- post-launch measurement and iteration;
- AI safety and human-control decisions in a financial context.
