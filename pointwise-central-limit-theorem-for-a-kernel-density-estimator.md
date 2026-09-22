# Pointwise central limit theorem for a kernel density estimator

↑ **Parent:** [Kernel density estimation](kernel-density-estimation.md)

Let the [kernel for density estimation](kernel-for-density-estimation.md) have integral one, be bounded and have compact support. For a [probability density function](probability-density-function.md) with bounded derivative, assume $h\to0$, $nh\to\infty$ and $nh^3\to0$. The [bias of a kernel density estimator](bias-of-a-kernel-density-estimator.md) is $O(h)$, negligible on the $\sqrt{nh}$ scale. For $Y_{n,i}=K((x-X_i)/h)$, $h^{-1}\operatorname{Var}Y_{n,i}\to f(x)\|K\|_2^2$. The centered summands divided by $\sqrt{nh}$ are uniformly small, so the [Lindeberg-Feller central limit theorem](lindeberg-feller-central-limit-theorem.md) applies. The condition $nh^3\to0$ alone is insufficient: with $h=n^{-2}$ and a compactly supported kernel, with probability tending to one no observation enters the kernel window, producing a degenerate limit at a point with positive density.

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

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-33/2/solution.md)
