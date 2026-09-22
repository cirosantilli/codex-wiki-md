# Randomized symmetric finite-difference derivative estimator

↑ **Parent:** [Finite difference](finite-difference-split.md)

Given noisy evaluations at $x_0+hZ_i$, where the $Z_i$ are independent [Rademacher random variables](rademacher-distribution.md), the estimator

$$
\widehat g'_N(x_0)=\frac1N\sum_{i=1}^N\frac{Z_i(Y_i-g(x_0))}{h}
$$

averages one-sided finite differences from both directions. If $|g''|\leq M$ and the noise variance is $\sigma^2$, its [mean squared error](mean-squared-error.md) is at most $h^2M^2/4+\sigma^2/(Nh^2)$.

## ↑ Ancestors (6)

1. [Finite difference](finite-difference-split.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-4/28k/c/solution.md)
