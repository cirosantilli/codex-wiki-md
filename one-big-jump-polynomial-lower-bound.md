# One-big-jump polynomial lower bound

↑ **Parent:** [Pareto distribution](pareto-distribution.md)

Let $S_n=\sum_{i=1}^nX_i$, where the summands are [independent and identically distributed](independent-and-identically-distributed-random-variables.md) with [Pareto distribution](pareto-distribution.md) $\operatorname{Pareto}(\alpha,\beta)$. Their positivity implies $\{X_1\geq na\}\subseteq\{S_n\geq na\}$, so for fixed $a>0$ and $na\geq\beta$,

$$
\mathbb P(S_n\geq na)\geq\left(\frac{\beta}{na}\right)^\alpha,\qquad
\frac{\alpha}{n}\log\frac{\beta}{na}\leq\frac1n\log\mathbb P(S_n\geq na)\leq0.
$$

Both outer expressions tend to zero. A single large summand already prevents a strictly negative exponential rate. No positive [exponential moment](exponential-moment.md) exists, so the exponential-moment form of the [Cramér theorem](cramer-s-theorem.md) cannot be applied. The bound proves this logarithmic rate and does not assert an exact tail asymptotic. In particular, it remains true when $a$ lies below a finite [mean](expected-value-split.md), where the event need not even be rare. The stronger fixed-summand-count asymptotic in a [heavy-tailed subexponential distribution](subexponential-distribution-heavy-tailed.md) is a separate statement.

## ↑ Ancestors (8)

1. [Pareto distribution](pareto-distribution.md)
2. [Continuous probability distribution](continuous-probability-distribution-split.md)
3. [Probability distribution](probability-distribution-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-33/2/c/solution.md)
