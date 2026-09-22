# Common-coin averaging

↑ **Parent:** [Independent and identically distributed random variables](independent-and-identically-distributed-random-variables.md)

In the copied-coin model, $X_i=Z$ for every $i$, so the [sample mean](sample-mean.md) is exactly $Z$, however large $n$ is. Its [expected value](expected-value-split.md) is $1/2$ and its [variance](variance-split.md) is $1/4$, matching each observation's marginal variance. The off-diagonal [covariances](covariance.md) in the [variance of a sum](variance-of-a-sum.md) explain the difference:

$$
\operatorname{Var}(\overline X)=\frac1{n^2}\sum_{i,j=1}^n\operatorname{Cov}(X_i,X_j)=\frac1{n^2}\sum_{i,j=1}^n\frac14=\frac14.
$$

For an [IID sample](independent-and-identically-distributed-random-variables.md), those off-diagonal terms are zero. Repeating the same random input therefore does not create the reduction in fluctuations obtained from fresh independent draws. The general common-plus-individual structure is described by [compound-symmetry covariance](compound-symmetry-covariance.md).

## ↑ Ancestors (8)

1. [Independent and identically distributed random variables](independent-and-identically-distributed-random-variables.md)
2. [Independent random variables](independent-random-variables.md)
3. [Random variable](random-variable-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Variance of a sample mean](variance-of-a-sample-mean.md)
