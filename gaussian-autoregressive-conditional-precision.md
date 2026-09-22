# Gaussian autoregressive conditional precision

↑ **Parent:** [Autoregressive process of order one](autoregressive-process-of-order-one.md)

For a stationary unit-variance [normal distribution](normal-distribution.md) autoregression with coefficient $a\in(-1,1)$, its vector of length $T\geq2$ has [precision matrix](precision-matrix.md) $J$ that is tridiagonal: the two endpoint diagonal entries are $1/(1-a^2)$, interior entries are $(1+a^2)/(1-a^2)$, and adjacent off-diagonal entries are $-a/(1-a^2)$. An independent observation $r=\lambda Z+\eta$, with covariance $vI$, updates precision and information vector to

$$
Q=J+\lambda^2v^{-1}I,\qquad h=\lambda v^{-1}r.
$$

The conditional law is [multivariate normal distribution](multivariate-normal-distribution.md) $N(Q^{-1}h,Q^{-1})$.

## ↑ Ancestors (8)

1. [Autoregressive process of order one](autoregressive-process-of-order-one.md)
2. [Autoregressive model](autoregressive-model.md)
3. [Autoregressive moving-average model](autoregressive-moving-average-model.md)
4. [Time series](time-series-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-216/3/b/i/solution.md)
