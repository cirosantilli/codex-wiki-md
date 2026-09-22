# Comparing a subgroup mean with its containing sample mean

↑ **Parent:** [Sample mean](sample-mean.md)

Partition a sample into two disjoint groups $A,B$ with fixed positive sizes $n_A,n_B$, and let $w=n_A/(n_A+n_B)$. The overall [sample mean](sample-mean.md) is the [weighted mean](weighted-arithmetic-mean.md)

$$
\overline X=w\overline X_A+(1-w)\overline X_B.
$$

Subtracting gives the displayed identity. The subgroup and overall [sample means](sample-mean.md) share observations, so they are not [independent](independent-random-variables.md). If the two disjoint groups are sampled [independently](independent-random-variables.md), then

$$
\operatorname{Cov}(\overline X_A,\overline X)=w\operatorname{Var}(\overline X_A),\qquad
\operatorname{Var}(\overline X_A-\overline X)=(1-w)^2\left\{\operatorname{Var}(\overline X_A)+\operatorname{Var}(\overline X_B)\right\}.
$$

Thus treating the subgroup and the combined sample as two [independent](independent-random-variables.md) samples uses the wrong [standard error](standard-error.md). Equality of the subgroup and overall population means is equivalent to equality of subgroup and complement means when both groups have positive weight, but the [sampling distribution](sampling-distribution.md) must respect the shared observations.

## ↑ Ancestors (11)

1. [Sample mean](sample-mean.md)
2. [Sample mean and covariance](sample-mean-and-covariance.md)
3. [Covariance matrix](covariance-matrix.md)
4. [Covariance](covariance.md)
5. [Variance](variance-split.md)
6. [Expected value](expected-value-split.md)
7. [Probability theory](probability-theory-split.md)
8. [Probability and statistics](probability-and-statistics-split.md)
9. [Area of mathematics](area-of-mathematics.md)
10. [Mathematics](mathematics-split.md)
11. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-digital-social-research-statistics-core-course-of-the-university-of-oxford/2023/1/solution.md)
