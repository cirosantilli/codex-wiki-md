# Cox rank-likelihood deletion consistency

↑ **Parent:** [Cox partial likelihood](cox-partial-likelihood.md)

Assume [independent](independent-random-variables.md) individual event times with positive time-constant [hazard multipliers](hazard-multiplier.md) and a common [baseline hazard](baseline-hazard.md) whose cumulative hazard tends to infinity. Transforming each event time by that cumulative hazard then gives [independent](independent-random-variables.md) exponential event times with corresponding rates, so all event orders exist. Their complete-order [probabilities](probability.md) select each next label proportionally to its remaining multiplier. Marginalizing over the position of a deleted label leaves the order law of the other exponential times, hence the same sequential formula without that label. This proves the deletion identity used when unobserved ranks are summed out. It does not supply a [likelihood function](likelihood-function.md) for censoring times; ignoring censoring in observed survival analysis still needs [independent censoring](independent-censoring.md).

## ↑ Ancestors (7)

1. [Cox partial likelihood](cox-partial-likelihood.md)
2. [Cox proportional-hazards model](cox-proportional-hazards-model.md)
3. [Survival analysis](survival-analysis-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-207/5/b/solution.md)
