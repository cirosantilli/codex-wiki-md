# Optimality of the Epanechnikov kernel

↑ **Parent:** [Epanechnikov kernel](epanechnikov-kernel.md)

Fix the second moment $v>0$. Put $B=\sqrt{5v}$ and $E(u)=3(B^2-u^2)_+/(4B^3)$. For every nonnegative unit-integral [kernel for density estimation](kernel-for-density-estimation.md) $K$ with the same second moment and finite $R(K)$, the mass and second-moment constraints give $\int(B^2-u^2)(K-E)=0$. Outside $[-B,B]$, $E=0$ and $(B^2-u^2)K\leq0$, so $\int E(K-E)\geq0$. Expanding the square gives $R(K)-R(E)=\int(K-E)^2+2\int E(K-E)\geq0$, with equality only when $K=E$ almost everywhere. Since $R(K)^2\mu_2(K)$ is scale invariant, rescaled [Epanechnikov kernels](epanechnikov-kernel.md) minimize the optimized [asymptotic mean integrated squared error](asymptotic-mean-integrated-squared-error.md) over all such second moments. This conclusion concerns nonnegative second-order kernels; signed higher-order kernels obey a different bias expansion.

## ↑ Ancestors (9)

1. [Epanechnikov kernel](epanechnikov-kernel.md)
2. [Kernel for density estimation](kernel-for-density-estimation.md)
3. [Density estimation](density-estimation.md)
4. [Nonparametric statistics](nonparametric-statistics-split.md)
5. [Statistical inference](statistical-inference-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-49/4/solution.md)
