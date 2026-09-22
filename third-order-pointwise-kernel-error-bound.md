# Third-order pointwise kernel error bound

↑ **Parent:** [Kernel density estimation](kernel-density-estimation.md)

Suppose a [probability density function](probability-density-function.md) and its third [derivative](derivative.md) are bounded. A square-integrable unit-integral [kernel for density estimation](kernel-for-density-estimation.md) with first two moments zero and $\mu_3=\int|u|^3|K(u)|du<\infty$ has [bias of a kernel density estimator](bias-of-a-kernel-density-estimator.md) at most $\|f^{(3)}\|_\infty\mu_3h^3/6$, by [Taylor theorem with Lagrange remainder](taylor-theorem-with-lagrange-remainder.md) and moment cancellation. Independence gives [variance](variance-split.md) at most $\|f\|_\infty\|K\|_2^2/(nh)$. The [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) bounds the expected centred absolute deviation by the square root of this variance. Adding the bias proves the inequality uniformly in $x$. The choice $h=n^{-1/7}$ gives expected absolute error $O(n^{-3/7})$.

## ↑ Ancestors (9)

1. [Kernel density estimation](kernel-density-estimation.md)
2. [Kernel for density estimation](kernel-for-density-estimation.md)
3. [Density estimation](density-estimation.md)
4. [Nonparametric statistics](nonparametric-statistics-split.md)
5. [Statistical inference](statistical-inference-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-31/2/solution.md)
