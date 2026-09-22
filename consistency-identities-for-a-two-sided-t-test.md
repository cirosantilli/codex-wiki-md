# Consistency identities for a two-sided t-test

↑ **Parent:** [Student's t-test](student-s-t-test.md)

For one two-sided t procedure with observed estimate $\widehat\Delta$, positive [standard error](standard-error.md) $s$, null value $\Delta_0$ and reference [Student t-distribution](student-s-t-distribution.md) with $\nu$ [statistical degrees of freedom](statistical-degrees-of-freedom.md), the [test statistic](test-statistic.md) and [p-value](p-value.md) must satisfy

$$
t=\frac{\widehat\Delta-\Delta_0}{s},\qquad p=2\{1-F_\nu(|t|)\}.
$$

Its symmetric [confidence interval](confidence-interval.md) at [coverage probability](coverage-probability.md) $1-\alpha$ is $[\widehat\Delta-t_{\nu,1-\alpha/2}s,\widehat\Delta+t_{\nu,1-\alpha/2}s]$ and therefore has midpoint $\widehat\Delta$. When the same [standard error](standard-error.md) and reference distribution are used, excluding $\Delta_0$ is equivalent to $|t|>t_{\nu,1-\alpha/2}$ and hence $p<\alpha$ for a continuous reference distribution. This proves the test–[interval](interval-mathematics.md) equivalence and supplies several [independent](independent-random-variables.md) checks on a printed output. An approximate [Welch's t-test](welch-s-t-test.md) uses its same approximate [statistical degrees of freedom](statistical-degrees-of-freedom.md) throughout. Rounding can blur a boundary decision but cannot explain a confidence-interval midpoint far from the reported estimate.

## ↑ Ancestors (8)

1. [Student's t-test](student-s-t-test.md)
2. [Statistical hypothesis test](statistical-hypothesis-test-split.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-digital-social-research-statistics-core-course-of-the-university-of-oxford/2020/1/solution.md)
