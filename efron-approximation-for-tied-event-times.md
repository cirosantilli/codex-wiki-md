# Efron approximation for tied event times

↑ **Parent:** [Cox partial likelihood](cox-partial-likelihood.md)

For $d$ events tied within a [risk set](risk-set.md), put $u_i=\exp(\beta^Tz_i)$, $S=\sum_{i\in R}u_i$ and $U_D=\sum_{i\in D}u_i$. The Efron approximation to [Cox partial likelihood](cox-partial-likelihood.md) removes the average tied-event [hazard multiplier](hazard-multiplier.md) from the denominator at each successive event. Unlike the [Breslow approximation for tied event times](breslow-approximation-for-tied-event-times.md), it accounts approximately for depletion of the [risk set](risk-set.md) within the group. Factors independent of $\beta$ can be dropped for estimation. This is an approximation for coarsened continuous event times, not a full interval-observation [likelihood](likelihood-function.md).

## ↑ Ancestors (7)

1. [Cox partial likelihood](cox-partial-likelihood.md)
2. [Cox proportional-hazards model](cox-proportional-hazards-model.md)
3. [Survival analysis](survival-analysis-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-41/3/b/solution.md)
