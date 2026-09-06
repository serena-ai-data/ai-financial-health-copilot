# Product Requirements — MVP

## Product
AI Financial Health Copilot

## Problem
Users may hold accounts, debt, insurance and investments across multiple providers but still lack a simple, consolidated understanding of their overall financial health and action priorities.

## Primary user
Working professionals who already use multiple financial products but are not financial specialists and want a clearer view of their overall financial position.

## Product goal
Help a user reach a useful first financial-health insight quickly, with transparent reasoning and clear uncertainty.

### Target metric
**Time to First Insight < 3 minutes** — a design target, not a measured result yet.

## MVP scope

### In scope
- synthetic demo profile;
- manual input for income, spending, liquidity, investments and short-term debt;
- simplified protection-status input;
- review and correction before analysis;
- deterministic calculations and score classification;
- weighted financial-health score;
- explainability view;
- prioritised action plan;
- locally simulated AI-copilot interaction;
- trust and compliance design concepts.

### Out of scope
- real bank connections;
- live payment or transfer execution;
- securities trading;
- insurance purchase;
- guaranteed investment recommendations;
- autonomous high-risk financial decisions;
- production-grade KYC, AML or suitability workflows;
- live LLM integration in the current public prototype.

## Core user stories

1. As a user, I want to enter my financial information so I can understand my overall position.
2. As a user, I want to review extracted or entered information before analysis so mistakes do not silently influence recommendations.
3. As a user, I want to understand why I received a score so I can evaluate the result.
4. As a user, I want recommendations ranked by priority so I know what to address first.
5. As a user, I want the system to express uncertainty when information is incomplete.

## Functional requirements

- FR-01: Load a synthetic demo profile.
- FR-02: Accept manual financial inputs.
- FR-03: Calculate monthly surplus and savings rate.
- FR-04: Calculate emergency-fund coverage.
- FR-05: Classify each dimension using deterministic rules.
- FR-06: Calculate an overall weighted score.
- FR-07: Display calculation logic and limitations.
- FR-08: Allow users to review/correct input before final analysis.
- FR-09: Produce prioritised next-step guidance.
- FR-10: Keep AI separate from balance, transaction-state and score calculation.
- FR-11: Preserve uncertainty rather than invent missing facts.

## Success metrics for future testing

- Financial Health Report completion rate
- Time to First Insight
- Input correction rate
- Source-attribution accuracy
- Unsupported-claim rate
- Unsafe-recommendation rate
- Percentage of completed reports with at least one reviewed action
