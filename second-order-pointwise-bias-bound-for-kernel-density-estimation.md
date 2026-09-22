# Second-order pointwise bias bound for kernel density estimation

↑ **Parent:** [Bias of a kernel density estimator](bias-of-a-kernel-density-estimator.md)

Let a nonnegative [kernel for density estimation](kernel-for-density-estimation.md) $K$ have integral one, zero first moment and finite second moment $\mu_2(K)$. If a [probability density function](probability-density-function.md) $f$ has bounded [second derivative](second-derivative.md), its [kernel density estimator](kernel-density-estimation.md) has pointwise [bias](bias-of-an-estimator.md) at most $h^2\mu_2(K)\|f^{\prime\prime}\|_\infty/2$. Apply the [Taylor theorem with Lagrange remainder](taylor-theorem-with-lagrange-remainder.md) to $f(x-hu)$ and integrate: the first-order term vanishes and the remainder is bounded by $h^2u^2\|f^{\prime\prime}\|_\infty/2$. For $K=\mathbb1_{[-1/2,1/2]}$, $\mu_2(K)=1/12$.

## ↑ Ancestors (10)

1. [Bias of a kernel density estimator](bias-of-a-kernel-density-estimator.md)
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

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-210/1/solution.md)
