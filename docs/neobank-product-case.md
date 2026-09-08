# AI Neobank Product Case

Independent portfolio case by Serena Qin. This document frames an AI-neobank product hypothesis around a narrow initial wedge: helping users turn fragmented financial information into an understandable overall position and a clear next action.

> **Claim boundary:** the Financial Health Copilot is the demonstrated interactive MVP. Connected accounts, payments, savings, insurance, investing and execution capabilities below are future product hypotheses, not shipped claims.

## 1. User problem

Users may hold money across bank accounts, cards, wallets, insurance and investments. Product-level information exists, but three cross-product questions remain difficult:

1. What is my overall financial position?
2. What matters most right now?
3. What should I do next?

The proposed neobank experience starts by creating a reusable decision layer across financial products rather than launching every financial capability at once.

## 2. Primary user

Working professionals who already use multiple financial products but are not financial specialists.

Key needs:
- one understandable financial picture;
- low-friction review of important facts;
- clear prioritisation rather than generic tips;
- visible reasoning and uncertainty;
- control over consequential financial actions.

## 3. Product thesis

**One financial picture. One clear next step.**

The product should first earn trust by helping users understand their money. Only after this value is proven should it expand into connected context, personalised actions and governed execution.

Core journey:

`Onboarding & consent -> Add / connect financial context -> Unified money view -> Financial health -> Priority action -> AI explanation -> Human-confirmed action`

## 4. Demonstrated MVP

The current live Financial Health Copilot demonstrates:

- consent and AI-boundary disclosure;
- structured financial input;
- review and correction;
- deterministic financial-health analysis;
- transparent scoring;
- prioritised next-best action;
- explainability;
- bounded AI Copilot interaction;
- synthetic data only.

The deterministic layer owns calculations and verified financial state. AI is used only for interpretation and explanation.

## 5. Future product hypotheses

### V2 — Connected financial context
- bank / wallet / insurance connectors where feasible;
- source-level traceability;
- recurring refresh;
- exception and data-quality handling.

### V3 — Personalised financial actions
- goal planning;
- contextual nudges;
- action ranking;
- deeper liquidity / protection analysis;
- experimentation framework.

### V4 — Governed execution
- user-confirmed payments or product hand-offs;
- suitability / eligibility controls where required;
- audit trails and approval logic;
- explicit limits on autonomous AI action.

## 6. MVP backlog

### P0 — Trust-critical path
- onboarding and consent;
- structured data input;
- review and correction;
- deterministic analysis;
- unified financial-health view.

### P1 — User value
- explainability;
- prioritised next-best action;
- clear uncertainty states.

### P2 — Intelligence and continuity
- bounded AI Copilot;
- connected financial data;
- recurring context refresh.

## 7. Product metrics

These are proposed future metrics, not claimed production results.

### Activation
- onboarding completion rate;
- financial-data completion rate;
- Time to First Insight;
- first-action review rate.

### Engagement
- next-best-action engagement;
- explainability usage;
- repeat usage / return rate;
- feature adoption by financial category.

### Retention and value
- 7-day / 30-day return rate;
- percentage of users with an updated financial picture;
- action follow-through rate;
- user-reported clarity / confidence.

### Trust and AI quality
- input correction rate;
- unsupported-claim rate;
- numerical-consistency rate;
- unsafe-recommendation rate;
- percentage of AI answers grounded in verified product state;
- escalation / human-review rate.

## 8. Experiment plan

### Experiment A — unified view vs category-first onboarding
Hypothesis: showing a cross-product financial picture earlier improves perceived value and completion.

Primary measure: Time to First Insight and completion rate.

### Experiment B — generic recommendations vs one prioritised action
Hypothesis: one ranked next action creates more engagement than a list of equally weighted tips.

Primary measure: action-review and follow-through rate.

### Experiment C — opaque AI explanation vs evidence-linked explanation
Hypothesis: visible facts, rules and uncertainty improve trust without materially reducing completion.

Primary measure: explainability usage, correction rate and user-reported confidence.

## 9. Product trade-offs

| Trade-off | MVP decision | Reasoning |
| --- | --- | --- |
| Breadth vs focus | Start with financial understanding | Validate a high-value cross-product problem before building a super-app |
| Connected data vs manual input | Start with manual / synthetic input | Prove value before investing in integrations |
| LLM score vs deterministic score | Deterministic score | Financial calculations need reproducibility and auditability |
| AI autonomy vs user control | Human-confirmed actions | Consequential financial actions require stronger safeguards |
| Speed vs perfect data | Bounded progress with visible uncertainty | Useful decisions are possible without pretending missing data does not exist |

## 10. Operating loop

`Production signal -> triage -> user/business impact -> root cause -> backlog priority -> release -> measurement -> iteration`

Priority rules:
- safety or material financial-state defects override roadmap work;
- high-frequency journey failures outrank low-usage feature expansion;
- low-adoption features are investigated before more complexity is added;
- AI behaviour that changes verified numbers or overstates certainty is release-blocking.

## 11. Localisation hypothesis

### China
Potential emphasis on cross-provider financial fragmentation, cross-insurer organisation, liquidity, accessibility, fraud/scam awareness, sensitive-data consent and explainable AI guidance.

### Southeast Asia
Depending on market: wallet-first journeys, remittance, accessible protection, financial inclusion, multicurrency needs, low-bandwidth experiences and local regulatory / religious-product considerations.

The platform logic can be shared, but the local user problem and operating constraints should drive prioritisation.

## 12. What this case demonstrates

- user-problem framing;
- product direction;
- MVP scoping;
- backlog prioritisation;
- financial-journey simplification;
- metrics and experimentation;
- post-launch iteration;
- AI boundaries and trust controls;
- roadmap trade-offs;
- localisation thinking.

## Disclaimer

This is an independent portfolio project. It is not affiliated with, endorsed by, or produced for BJAK or any financial institution. It is not financial, legal or investment advice.