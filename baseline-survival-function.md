# Baseline survival function

↑ **Parent:** [Proportional hazards model](proportional-hazards-model.md)

In a [proportional hazards model](proportional-hazards-model.md) $h(t\mid z)=h_0(t)e^{\beta^Tz}$, the [baseline survival function](baseline-survival-function.md) is $S_0(t)=\exp\{-\int_0^t h_0(u)\,du\}$, corresponding to the reference covariate vector $z=0$. Integrating the [hazard function](hazard-function.md) gives $S(t\mid z)=S_0(t)^{e^{\beta^Tz}}$. Estimated [hazard ratios](hazard-ratio.md) alone therefore do not determine absolute survival probabilities: the [baseline hazard](baseline-hazard.md) or [baseline survival function](baseline-survival-function.md) must also be estimated.

## ↑ Ancestors (6)

1. [Proportional hazards model](proportional-hazards-model.md)
2. [Survival analysis](survival-analysis-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Baseline survival function](baseline-survival-function.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-41/5/b/ii/solution.md)
