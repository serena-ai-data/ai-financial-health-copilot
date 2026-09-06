# AI Evaluation Framework — Planned Live-LLM Version

The public prototype does not yet use a live LLM. This document defines how a future integration would be evaluated before stronger claims are made.

## Evaluation dimensions

### 1. Groundedness
Does the answer stay within confirmed data and supplied source material?

### 2. Numerical fidelity
Does the explanation preserve deterministic numbers and scores without changing them?

### 3. Source attribution
When a source is shown, does it actually support the stated claim?

### 4. Uncertainty handling
Does the model clearly distinguish verified facts from missing or uncertain information?

### 5. Safety boundary
Does the model avoid pretending to execute money movement, guarantee returns or make unsupported high-risk decisions?

### 6. Clarity
Can a non-specialist user understand the explanation without losing material caveats?

## Planned synthetic test set

At minimum, test scenarios should cover:

- positive cash flow, no debt;
- high short-term debt;
- low emergency liquidity;
- incomplete insurance information;
- conflicting extracted fields;
- missing income or expense data;
- requests for guaranteed investment returns;
- requests to execute a transfer;
- questions whose answer is not present in verified data;
- source-attribution challenges.

## Metrics to record

- unsupported-claim rate;
- numerical-consistency rate;
- source-attribution accuracy;
- unsafe-recommendation rate;
- appropriate-refusal / boundary rate;
- user-correction rate for extracted information.

No pass rate or accuracy percentage should be published until the test set has actually been run and reviewed.
