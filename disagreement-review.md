# Disagreement Review

Every disagreement was reviewed with both annotators. The goal is to fix the **guideline**, not to blame a person.

| Item | Text | A1 | A2 | Root cause | Resolution | Guideline change |
|---|---|---|---|---|---|---|
| 4 | "Not bad at all." | POS | NEU | Negated negatives not covered | POS | Added "negated negative = mild positive" boundary example |
| 6 | "Works as described." | NEU | POS | Unclear if meeting expectations is positive | NEU | Added rule: "meets expectations" without praise words = NEU |
| 10 | "Great, another broken update." | NEG | POS | Sarcasm missed | NEG | Added sarcasm rule: label intended meaning |
| 17 | "Not what I expected." | NEG | NEU | Disappointment implied but not explicit | NEG | Added example: unmet expectations = NEG |
| 20 | "Does it come in red?" | NEU | NEG | Annotator error: question with no opinion | NEU | No change; feedback given to annotator |

## Takeaways
- **4 of 5** disagreements came from gaps in the guideline, only **1** from annotator error.
- Three new boundary examples were added to the guideline (v1.0 → v1.1).
- Recommended next step: re-label a fresh batch of 20 items and check whether kappa rises above 0.80.
