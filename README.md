# Inter-Annotator Agreement — Worked Example

A step-by-step walkthrough of how to measure whether annotators are labeling consistently, using **percent agreement** and **Cohen's kappa** on a small synthetic dataset.

> The labels in this repo are **synthetic** and created for demonstration.

## Why it matters
If two trained annotators can't agree on a label, a model can't learn it reliably. Agreement metrics show **where the guideline is unclear**, not just who made mistakes.

## Contents
| File | Purpose |
|---|---|
| [`data/two_annotator_labels.csv`](data/two_annotator_labels.csv) | 20 items labeled independently by two annotators |
| [`worked-calculation.md`](worked-calculation.md) | Full hand calculation of percent agreement and Cohen's kappa |
| [`disagreement-review.md`](disagreement-review.md) | Analysis of each disagreement and the guideline fixes it led to |

## Results at a glance
| Metric | Value |
|---|---|
| Items | 20 |
| Percent agreement | 75% |
| Cohen's kappa | 0.62 (substantial) |

## Interpreting kappa (Landis & Koch, 1977)
| κ | Agreement |
|---|---|
| < 0.00 | Poor |
| 0.00–0.20 | Slight |
| 0.21–0.40 | Fair |
| 0.41–0.60 | Moderate |
| 0.61–0.80 | Substantial |
| 0.81–1.00 | Almost perfect |

## License
MIT
