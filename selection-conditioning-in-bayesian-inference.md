# Selection conditioning in Bayesian inference

↑ **Parent:** [Bayesian statistics](bayesian-statistics-split.md)

If inclusion depends only on fully observed data $d$, then $p(S\mid d,\theta)=p(S\mid d)$ cancels from [Bayes' theorem](bayes-theorem.md) for that individual's parameters. Selection can still matter for unknown population parameters and for missing or unconditioned features. For independent detected observations conditional on their count and population parameters $\Lambda$, each [likelihood](likelihood-function.md) has normalization $\alpha(\Lambda)=\int S(d)p(d\mid\Lambda)\,dd$. A model for the detected count adds its own count [likelihood](likelihood-function.md). Do not combine a selected-population [prior](prior-probability.md) with a truncated-data [likelihood](likelihood-function.md) in a way that counts the same selection twice.

## ↑ Ancestors (6)

1. [Bayesian statistics](bayesian-statistics-split.md)
2. [Statistical inference](statistical-inference-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-frontiers-of-observational-astrophysics-course-of-the-university-of-cambridge/2014/paper-1/2/solution.md)
