# Duality between confidence intervals and hypothesis tests

↑ **Parent:** [Confidence interval](confidence-interval.md)

Invert a family of [hypothesis tests](statistical-hypothesis-test-split.md) by including each parameter value in the [confidence set](confidence-region.md) exactly when its test does not reject. For any true value $\theta$, the events $\{\theta\notin C(X)\}$ and $\{\text{reject }H_\theta\}$ are identical. Thus size at most $\alpha$ gives coverage at least $1-\alpha$, and exact size gives exact coverage. When the accepted set is an interval, this is a [confidence interval](confidence-interval.md).

For the normal sample mean with unknown variance, the central [Student t-distribution](student-s-t-distribution.md) interval excludes zero exactly when $|\sqrt n\,\overline X/S|$ exceeds the same two-sided critical quantile. A two-sided [p-value](p-value.md) strictly below $\alpha$ therefore implies exclusion of zero from the matching closed interval. Boundary conventions agree up to events of probability zero in this continuous model.

## ↑ Ancestors (6)

1. [Confidence interval](confidence-interval.md)
2. [Statistical inference](statistical-inference-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-options-i-course-of-the-university-of-oxford/2010/o/o1/b/solution.md)
- [Solution](past-exam-of-the-probability-statistics-and-options-i-course-of-the-university-of-oxford/2011/o/3/d/solution.md)
