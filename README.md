# AI Financial Health Copilot

An independent AI FinTech product case study exploring how fragmented financial information can be turned into understandable, prioritised and explainable next-step guidance.

> **Status:** public product prototype. The current demo uses synthetic data and deterministic scoring rules. The AI Copilot interaction is locally simulated and is **not yet connected to a live LLM API**.

## Portfolio cases

This repository now contains two related but distinct product cases:

### 1. AI Financial Health Copilot
A live, deeper MVP focused on financial understanding, deterministic scoring, explainability, next-best-action design and trust controls.

- Product case: `index.html`
- Interactive demo: `demo/`

### 2. AI Neobank Product Case
A China-market Product Manager case that expands the scope from financial-health decision support into a broader cross-product neobank journey across banking, cards, insurance and investments.

- Product case: `neobank/index.html`
- Interactive concept app: `neobank/app.html`

The AI Neobank case extends the product scope into a broader cross-product journey, while the Financial Health Copilot remains the deeper implemented MVP module and execution evidence.

## Product idea

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

## Core flow

`Welcome -> Consent -> Add data -> Review & verify -> Analyse -> Dashboard -> Explainability -> Action plan -> AI Copilot`

## Product-owner view

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

## System boundary

`User / financial source -> validation & review -> deterministic rules engine -> financial state -> AI explanation layer -> user interface`

The deterministic layer remains the source of truth for confirmed financial facts, calculations, score classification and transaction state. The AI layer may interpret and explain verified information, surface uncertainty and answer grounded questions, but it must not silently alter balances, verified facts or score calculations.

## Why deterministic rules matter

Financial states and numerical calculations need consistency and auditability. In this prototype, calculations and score classification are deterministic. AI is positioned as an interpretation and explanation layer rather than the source of truth for balances, transaction states or financial facts.

## Trust & compliance design

The product includes concepts such as:

- consent before sensitive-data collection;
- source traceability for extracted information;
- user correction before AI-derived data influences analysis;
- visible uncertainty instead of false precision;
- audit-trail thinking for material changes;
- human verification for uncertain or consequential conclusions;
- clear boundaries between AI assistance and financial execution.

## Proposed release path

### MVP — Financial understanding
Manual or synthetic input, review, deterministic analysis, explainability, prioritised next-best action and a bounded Copilot interaction.

### V2 — Connected financial context
Bank / wallet / insurance data connectors where legally and technically feasible, with source-level traceability and stronger exception handling.

### V3 — Personalised financial actions
Goal planning, context-aware nudges, deeper protection and liquidity analysis, and experimentation around action ranking.

### V4 — Governed execution
Human-confirmed transaction or product hand-off, stronger suitability / eligibility controls, audit trails and explicit limits on autonomous AI execution.

## Proposed post-launch metrics

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

## Demo data

The repository contains synthetic user data only. No real bank credentials, account numbers, policies, customer information or transaction data are used.

## Repository structure

- `index.html` — AI Financial Health Copilot product case-study website
- `demo/` — live Financial Health Copilot interactive prototype
- `neobank/` — AI Neobank Product Case and interactive China-market concept app
- `docs/product-requirements.md` — MVP scope and requirements
- `docs/product-ownership.md` — backlog, acceptance criteria, system boundary, roadmap, trade-offs and launch plan
- `docs/scoring-methodology.md` — deterministic scoring logic
- `docs/ai-safety-and-trust.md` — AI boundaries and trust design
- `docs/market-localisation.md` — China and Southeast Asia localisation hypotheses
- `docs/ai-evaluation.md` — evaluation framework for a future live-LLM version
- `data/synthetic-demo-data.json` — synthetic test profile

## Product ownership

Independent product case study by **Serena Qin**. Product strategy, workflow design, scoring logic, trust-and-compliance framework, prototype design, product-delivery planning and evaluation framework were developed for portfolio purposes.

## Disclaimer

This project is an independent portfolio project and is not affiliated with, endorsed by, or produced for BJAK or any financial institution. It is not financial, legal or investment advice.