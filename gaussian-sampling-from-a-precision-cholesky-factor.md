# Gaussian sampling from a precision Cholesky factor

↑ **Parent:** [Precision matrix](precision-matrix.md)

If a [positive-definite matrix](positive-definite-matrix.md) $Q=LL^T$ is the [precision matrix](precision-matrix.md) of a [multivariate normal distribution](multivariate-normal-distribution.md), draw independent $\xi\sim N(0,I)$ and solve $L^T\eta=\xi$. Then $m+\eta$ has covariance $L^{-T}L^{-1}=Q^{-1}$. This avoids forming the inverse and exploits a banded [Cholesky decomposition](cholesky-decomposition.md) when $Q$ is banded.

## ↑ Ancestors (10)

1. [Precision matrix](precision-matrix.md)
2. [Covariance matrix](covariance-matrix.md)
3. [Covariance](covariance.md)
4. [Variance](variance-split.md)
5. [Expected value](expected-value.md)
6. [Probability theory](probability-theory-split.md)
7. [Probability and statistics](probability-and-statistics-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-216/3/b/i/solution.md)
