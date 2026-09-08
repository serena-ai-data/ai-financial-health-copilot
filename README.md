# Serena — AI Product Portfolio

Independent AI product portfolio focused on **agentic workflows, FinTech, onboarding, UX, product delivery and AI evaluation**.

## Portfolio entry

- **Portfolio landing page:** `portfolio/index.html`
- **Central AI onboarding redesign:** `central-ai-onboarding/`
- **ApplyFlow AI application-operations assistant:** `applyflow/`
- **AI Financial Health Copilot:** `index.html`
- **AI Neobank / BJAK-oriented extension:** `neobank/`

> All cases are independent portfolio projects. They are not claimed as employer work or production outcomes. Synthetic data is used where appropriate.

---

## Case 1 — Central AI Onboarding Redesign

A targeted, hypothesis-driven case exploring how an AI business platform could move a new SMB user from signup to a first successful AI action faster.

**Demonstrates:**
- onboarding and UX thinking;
- activation funnel design;
- prioritisation;
- mini PRD and acceptance criteria;
- product metrics;
- interactive prototype.

This case is **not affiliated with or endorsed by Wing / Central AI**. No internal user data or production conversion metrics are claimed.

---

## Case 2 — ApplyFlow AI

An AI application-operations assistant inspired by real workflow complexity in education consulting, but built entirely with **synthetic applicant names and data** for portfolio purposes.

The product concept combines:
- applicant status;
- document completeness;
- deadlines;
- risk prioritisation;
- natural-language querying;
- next-best-action recommendations;
- human-approved follow-up tasks.

**Core principle:** AI may summarise, prioritise and recommend, but structured applicant records remain the source of truth.

---

## Case 3 — AI Financial Health Copilot

A deeper AI FinTech product case exploring how fragmented financial information can be turned into understandable, prioritised and explainable next-step guidance.

> **Status:** public product prototype. The current demo uses synthetic data and deterministic scoring rules. The AI Copilot interaction is locally simulated and is **not yet connected to a live LLM API**.

### Product idea

Many users hold financial products across different providers: bank accounts, credit cards, insurance policies and investments. Individual apps show product-level information, but users may still struggle to understand their overall financial position and decide what deserves attention first.

AI Financial Health Copilot is designed around a simple principle:

**AI explains. Rules calculate. Users stay in control.**

The MVP combines:
- structured financial input;
- deterministic calculations and scoring;
- review-and-verify steps before analysis;
- prioritised next-best actions;
- explainability for each score;
- a trust layer covering consent, uncertainty, traceability and auditability.

### Core flow

`Welcome -> Consent -> Add data -> Review & verify -> Analyse -> Dashboard -> Explainability -> Action plan -> AI Copilot`

### Product-owner view

This project is deliberately documented beyond a concept deck. The repository includes the product artefacts needed to show how the MVP could move from problem framing into engineering delivery and post-launch iteration:

- MVP scope and explicit out-of-scope decisions;
- core user stories and functional requirements;
- prioritised backlog;
- acceptance criteria and edge cases;
- engineering-facing system boundaries;
- release roadmap;
- product trade-offs;
- launch and post-launch measurement plan;
- AI evaluation and safety boundaries.

See `docs/product-ownership.md` for the technical product ownership and delivery plan.

### System boundary

`User / financial source -> validation & review -> deterministic rules engine -> financial state -> AI explanation layer -> user interface`

The deterministic layer remains the source of truth for confirmed financial facts, calculations, score classification and transaction state. The AI layer may interpret and explain verified information, surface uncertainty and answer grounded questions, but it must not silently alter balances, verified facts or score calculations.

### Trust & compliance design

The product includes concepts such as:
- consent before sensitive-data collection;
- source traceability for extracted information;
- user correction before AI-derived data influences analysis;
- visible uncertainty instead of false precision;
- audit-trail thinking for material changes;
- human verification for uncertain or consequential conclusions;
- clear boundaries between AI assistance and financial execution.

### Proposed post-launch metrics

These are design metrics for future testing, not claimed production results.

- financial-health report completion rate;
- Time to First Insight;
- step-level drop-off rate;
- repeat usage;
- input correction rate;
- explainability / next-best-action adoption;
- unsupported-claim rate;
- numerical-consistency rate;
- unsafe-recommendation rate;
- user-reported clarity / confidence;
- escalation rate in a production workflow.

---

## Product ownership

Independent product portfolio by **Serena Qin**. Product strategy, workflow design, trust-and-compliance thinking, prototypes, product-delivery planning and evaluation frameworks were developed for portfolio purposes.

## Privacy and data disclaimer

No real bank credentials, account numbers, policies, customer records or applicant records are used in the public portfolio demos. ApplyFlow applicant names and records are synthetic.

## General disclaimer

These projects are independent portfolio work and are not financial, legal, admissions or investment advice. Brand-targeted cases are not affiliated with, endorsed by, or produced for the referenced companies.