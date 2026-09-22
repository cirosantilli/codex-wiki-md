# Profile likelihood for a common Poisson rate ratio with unequal exposures

↑ **Parent:** [Poisson regression](poisson-regression.md)

For [independent](independent-random-variables.md) counts with means $p_{i1}\lambda_i$ and $p_{i2}\lambda_i r$, let $t_i=y_{i1}+y_{i2}$. Maximizing the [Poisson regression](poisson-regression.md) [likelihood](likelihood-function.md) in each baseline rate gives the displayed estimate. The remaining log-rate-ratio score is

$$
\sum_i\left[y_{i2}-\frac{t_i r p_{i2}}{p_{i1}+rp_{i2}}\right]=0.
$$

Equivalently, conditional on $t_i$, the second count has a [binomial distribution](binomial-distribution.md) with success [probability](probability.md) $rp_{i2}/(p_{i1}+rp_{i2})$. Each positive-total term increases strictly with $r$; if both treatment totals are positive, the score has a unique positive root. This reduces a many-parameter fit to a scalar equation.

## ↑ Ancestors (8)

1. [Poisson regression](poisson-regression.md)
2. [Generalized linear model](generalized-linear-model.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-36/3/i/solution.md)
