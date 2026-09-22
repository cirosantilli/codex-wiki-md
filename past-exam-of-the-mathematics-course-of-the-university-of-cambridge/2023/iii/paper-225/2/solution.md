<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $(\lambda_j,\phi_j)$ be the ordered eigenpairs of the common [covariance operator](../../../../../covariance-operator.md) $C_X$, and write $\delta=\mu-\mu^*$. Estimate $C_X$ by the [pooled covariance operator](../../../../../pooled-covariance-operator.md)

$$
\widehat C
=\frac1{2n}\sum_{i=1}^n\left[
(X_i-\overline X)\otimes(X_i-\overline X)
+(X_i^*-\overline X^*)\otimes(X_i^*-\overline X^*)
\right]
$$

and denote its first $K$ eigenpairs by $(\widehat\lambda_j,\widehat\phi_j)$. The sign ambiguity of each eigenfunction disappears after squaring. Consider the [Two-sample FPCA mean statistic](../../../../../two-sample-fpca-mean-statistic.md)

$$
T_{n,K}=\frac n2\sum_{j=1}^K
\frac{\langle\overline X-\overline X^*,\widehat\phi_j\rangle^2}
{\widehat\lambda_j}.
$$

Under $H_0$, the [Hilbert-space central limit theorem](../../../../../hilbert-space-central-limit-theorem.md) gives

$$
\sqrt{\frac n2}(\overline X-\overline X^*)
\xrightarrow{d}G,
$$

where $G$ is a centered [Gaussian random element](../../../../../gaussian-random-element.md) with covariance $C_X$. The assumed eigenvalue gaps give consistency of the estimated eigenvalues and eigenfunctions, so [Slutsky's theorem](../../../../../slutsky-theorem.md) yields

$$
T_{n,K}\xrightarrow{d}\sum_{j=1}^K
\frac{\langle G,\phi_j\rangle^2}{\lambda_j}
\sim\chi_K^2.
$$

An asymptotic level-$\alpha$ test therefore rejects when $T_{n,K}$ exceeds the $(1-\alpha)$-quantile of the [chi-squared distribution](../../../../../chi-squared-distribution.md) with $K$ degrees of freedom.

Under a fixed alternative,

$$
\frac{T_{n,K}}n\xrightarrow{p}
\frac12\sum_{j=1}^K\frac{\langle\delta,\phi_j\rangle^2}{\lambda_j}.
$$

The test is consequently consistent whenever the mean difference has a nonzero projection onto one of the retained principal components. A difference orthogonal to their span is invisible to this fixed-$K$ test, so $\mu\ne\mu^*$ alone does not guarantee consistency. Increasing $K$ with $n$ can recover such alternatives, but requires additional eigenvalue and approximation control.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 225](../../paper-225-split.md)
3. [Iii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
