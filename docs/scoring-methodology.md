# Scoring Methodology — Demo V1

The current scoring model is a transparent prototype model. It is **not** an industry standard and does not claim to determine a person's objective financial wellbeing.

## Overall score

`Financial Health Score = Cash Flow x 30% + Emergency Reserve x 25% + Debt x 25% + Protection x 20%`

## 1. Cash Flow — 30%

Savings rate:

`(monthly income - monthly spending) / monthly income`

| Savings rate | Demo score |
| --- | ---: |
| < 0% | 10 |
| 0–10% | 40 |
| 10–20% | 70 |
| >= 20% | 90 |

## 2. Emergency Reserve — 25%

Coverage:

`cash savings / essential monthly expenses`

| Coverage | Demo score |
| --- | ---: |
| < 1 month | 10 |
| 1–3 months | 40 |
| 3–6 months | 75 |
| >= 6 months | 100 |

## 3. Short-Term Debt — 25%

Ratio:

`credit-card balance / monthly income`

| Ratio | Demo score |
| --- | ---: |
| 0 | 100 |
| <= 0.5x | 70 |
| 0.5–1.0x | 40 |
| > 1.0x | 20 |

### Important limitation
A reported credit-card balance is not automatically high-cost debt. Interest status, due date, repayment behaviour and other context matter. The prototype therefore flags context as unknown rather than claiming that every balance is expensive debt.

## 4. Protection — 20%

The current MVP intentionally measures **information completeness / verification status**, not whether a user owns an objectively correct amount of insurance.

| Data status | Demo score |
| --- | ---: |
| Key information verified | 100 |
| Important fields need review | 70 |
| Material gap identified | 40 |
| Insufficient information | 20 |

## Example synthetic profile

The bundled Emma profile produces:

- Cash Flow: 90
- Emergency Reserve: 40
- Debt: 40
- Protection: 70

Weighted result: **61 / 100**.

The score is designed to be explainable: users can inspect the inputs, formula, rule and known limitations behind each dimension.
