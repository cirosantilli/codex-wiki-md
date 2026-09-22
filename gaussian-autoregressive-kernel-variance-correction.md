# Gaussian autoregressive kernel variance correction

↑ **Parent:** [Integrated variance of a kernel density estimator](integrated-variance-of-a-kernel-density-estimator.md)

For a stationary [autoregressive process of order one](autoregressive-process-of-order-one.md) with unit-variance [normal distribution](normal-distribution.md) marginals and fixed $0<\rho<1$, the [Gaussian kernel](gaussian-kernel.md) covariance correction at lag $j$ has the displayed form. The difference of two observations has variance $2(1-\rho^j)$, and their [characteristic functions](characteristic-function.md) reduce the Fourier integral to the difference of two [Gaussian integrals](gaussian-integral.md). The [mean value theorem](mean-value-theorem.md) gives $0\leq g_h(j)\leq\sqrt\pi\rho^j/[2(1-\rho)^{3/2}]$, uniformly over $h>0$. Thus the integrated variance differs from its independent-sample counterpart by $O(n^{-1})$. The marginal bias is unchanged, so this dependence does not alter the leading optimal bandwidth or the $n^{-4/5}$ [mean integrated squared error](integrated-mean-squared-error.md) for a second-order density kernel.

## ↑ Ancestors (10)

1. [Integrated variance of a kernel density estimator](integrated-variance-of-a-kernel-density-estimator.md)
2. [Kernel density estimation](kernel-density-estimation.md)
3. [Kernel for density estimation](kernel-for-density-estimation.md)
4. [Density estimation](density-estimation.md)
5. [Nonparametric statistics](nonparametric-statistics-split.md)
6. [Statistical inference](statistical-inference-split.md)
7. [Probability and statistics](probability-and-statistics-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-42/3/solution.md)
