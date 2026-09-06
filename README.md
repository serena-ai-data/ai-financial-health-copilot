# AI Financial Health Copilot

An independent AI FinTech product case study exploring how fragmented financial information can be turned into understandable, prioritised and explainable next-step guidance.

> **Status:** public product prototype. The current demo uses synthetic data and deterministic scoring rules. The AI Copilot interaction is locally simulated and is **not yet connected to a live LLM API**.

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

## Demo data

The repository contains synthetic user data only. No real bank credentials, account numbers, policies, customer information or transaction data are used.

## Repository structure

- `index.html` — product case-study website
- `demo/` — interactive product prototype
- `docs/product-requirements.md` — MVP scope and requirements
- `docs/scoring-methodology.md` — deterministic scoring logic
- `docs/ai-safety-and-trust.md` — AI boundaries and trust design
- `docs/market-localisation.md` — China and Southeast Asia localisation hypotheses
- `docs/ai-evaluation.md` — evaluation framework for a future live-LLM version
- `data/synthetic-demo-data.json` — synthetic test profile

## Product ownership

Independent product case study by **Serena Qin**. Product strategy, workflow design, scoring logic, trust-and-compliance framework, prototype design and evaluation planning were developed for portfolio purposes.

## Disclaimer

This project is an independent portfolio project and is not affiliated with, endorsed by, or produced for BJAK or any financial institution. It is not financial, legal or investment advice.
