# AI Safety & Trust Design

The product treats trust as part of the core financial-product experience rather than a legal notice added at the end.

## Principle

**AI explains. Deterministic systems calculate. Users stay in control.**

## AI can

- explain verified results in plain language;
- summarise complex financial documents;
- compare verified policy information;
- answer questions grounded in confirmed data;
- surface uncertainty and missing context;
- point users back to source information.

## AI must not

- invent financial data;
- alter balances or transaction states;
- guarantee investment returns;
- present uncertain information as verified fact;
- silently convert extracted content into a consequential recommendation;
- execute a transaction simply because a conversational model suggested it.

## Review-and-verify layer

A future document-ingestion flow should follow:

`AI extraction -> visible source -> confidence / uncertainty -> user correction -> confirmed data -> analysis`

AI extraction is therefore treated as a proposed interpretation, not automatically as ground truth.

## Explainability pattern

Each material result should be able to expose:

1. **Fact** — which confirmed inputs were used?
2. **Rule** — what calculation or policy was applied?
3. **Application** — how did the rule use those facts?
4. **Conclusion** — what did the product surface to the user?
5. **Uncertainty** — what important context is still unknown?

This structure is intentionally influenced by legal reasoning and auditability.

## Auditability

For consequential flows, the system design should preserve enough information to reconstruct what happened, including:

- original extracted value;
- user-corrected value;
- confirmed data used by the scoring engine;
- rule version;
- generated explanation;
- user confirmation or escalation.

## Privacy approach for this portfolio version

The public demo uses synthetic data only and does not request real credentials, bank logins or production financial records.
