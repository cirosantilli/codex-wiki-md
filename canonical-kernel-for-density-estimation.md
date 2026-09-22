# Canonical kernel for density estimation

↑ **Parent:** [Kernel density estimation](kernel-density-estimation.md)

For a nonnegative symmetric unit-integral [kernel for density estimation](kernel-for-density-estimation.md) with $0<\mu_2(K)=\int u^2K(u)\,du<\infty$ and $R(K)=\int K^2<\infty$, the canonical scaling satisfies $R(K_c)=\mu_2(K_c)^2$. Since $R(K_c)=R(K)/c$ and $\mu_2(K_c)=c^2\mu_2(K)$, the unique scale is $c=[R(K)/\mu_2(K)^2]^{1/5}$. Consequently its [asymptotic mean integrated squared error](asymptotic-mean-integrated-squared-error.md) is $C(K)[(nh)^{-1}+h^4R(f^{\prime\prime})/4]$, where $C(K)=R(K)^{4/5}\mu_2(K)^{2/5}$ is invariant under kernel rescaling. The leading optimal [smoothing bandwidth](smoothing-bandwidth.md) becomes $[nR(f^{\prime\prime})]^{-1/5}$, independent of the kernel shape. Unit second moment is a different normalization and does not have this separation property.

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

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-49/4/solution.md)
