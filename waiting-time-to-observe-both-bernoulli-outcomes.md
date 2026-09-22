# Waiting time to observe both Bernoulli outcomes

↑ **Parent:** [Coupon collector problem](coupon-collector-problem.md)

In independent trials with two outcomes of [probabilities](probability.md) $p$ and $q=1-p$, let $N$ include the first trial and the trial that first completes the pair. Conditional on the first outcome, $N-1$ has a [geometric distribution](geometric-distribution.md) of parameter $q$ or $p$, with mixture weights $p,q$. The [law of total expectation](law-of-total-expectation.md) and [law of total variance](law-of-total-variance.md) give

$$
EN=1+\frac pq+\frac qp=\frac1{pq}-1,\qquad
\operatorname{Var}N=\frac{p^2}{q^2}+\frac{q^2}{p^2}+\frac{(p-q)^2}{pq}
=\frac1{p^2q^2}-\frac3{pq}-2.
$$

The final term in the unsimplified variance is the [variance](variance-split.md) of the two conditional means; omitting it is incorrect unless $p=q$. Both outcomes must have positive [probability](probability.md) for these finite formulas.

## ↑ Ancestors (9)

1. [Coupon collector problem](coupon-collector-problem.md)
2. [Geometric distribution](geometric-distribution.md)
3. [Discrete probability distribution](discrete-probability-distribution-split.md)
4. [Probability distribution](probability-distribution.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-2/9f/b/solution.md)
