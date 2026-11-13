# Worked Calculation

Data: [`data/two_annotator_labels.csv`](data/two_annotator_labels.csv) (20 items, labels POS / NEU / NEG).

## 1. Confusion matrix

Rows = Annotator 1, columns = Annotator 2.

|            | POS | NEU | NEG | **Total A1** |
|---|---|---|---|---|
| **POS**    | 6 | 1 | 0 | **7** |
| **NEU**    | 1 | 4 | 1 | **6** |
| **NEG**    | 1 | 1 | 5 | **7** |
| **Total A2** | **8** | **6** | **6** | **20** |

Agreements are on the diagonal: 6 + 4 + 5 = **15**.

## 2. Observed agreement (pₒ)

pₒ = 15 / 20 = **0.75** (75%)

## 3. Expected agreement by chance (pₑ)

For each label: (A1 total / N) × (A2 total / N)

| Label | A1 share | A2 share | Product |
|---|---|---|---|
| POS | 7/20 = 0.35 | 8/20 = 0.40 | 0.140 |
| NEU | 6/20 = 0.30 | 6/20 = 0.30 | 0.090 |
| NEG | 7/20 = 0.35 | 6/20 = 0.30 | 0.105 |
| | | **pₑ** | **0.335** |

## 4. Cohen's kappa

κ = (pₒ − pₑ) / (1 − pₑ)
κ = (0.75 − 0.335) / (1 − 0.335)
κ = 0.415 / 0.665
κ ≈ **0.62** → *substantial agreement*

## 5. Why kappa instead of just 75%?
With three labels, two annotators labeling at their own rates would agree about 34% of the time by chance alone. Kappa removes that chance agreement, so 0.62 tells us how much **better than chance** the annotators are.
