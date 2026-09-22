<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let

$$
\overline C=\frac12(C_X+C_{X^*}),
\qquad
\overline C\phi_k=\lambda_k\phi_k,
$$

and estimate it by the average of the two within-sample [empirical covariance operators](../../../../../empirical-covariance-operator.md). Let $(\widehat\lambda_k,\widehat\phi_k)$ be its leading empirical eigenpairs and let $\overline X_n,\overline X_n^*$ be the sample means. Use the [Two-sample FPCA mean statistic](../../../../../two-sample-fpca-mean-statistic.md)

$$
\boxed{
T_{n,K}=\frac n2\sum_{k=1}^K
\frac{\langle\overline X_n-\overline X_n^*,\widehat\phi_k\rangle^2}
{\widehat\lambda_k}}.
$$

Under $H_0$, the [Hilbert-space central limit theorem](../../../../../hilbert-space-central-limit-theorem.md) gives

$$
\sqrt{\frac n2}(\overline X_n-\overline X_n^*)
\xrightarrow dG,
$$

where $G$ is a centered [Gaussian random element](../../../../../gaussian-random-element.md) with covariance $\overline C$. Distinct eigenvalues give consistent empirical eigenpairs, up to signs, and the standardized leading scores are independent standard normal variables. Hence

$$
T_{n,K}\xrightarrow d\chi_K^2.
$$

Rejecting above the $(1-\alpha)$ quantile gives an asymptotic level-$\alpha$ test.

Under a fixed alternative $\delta=\mu-\mu^*$,

$$
\frac{T_{n,K}}n\xrightarrow p
\frac12\sum_{k=1}^K\frac{\langle\delta,\phi_k\rangle^2}{\lambda_k}.
$$

The test is consistent whenever one retained projection is nonzero. Alternatives orthogonal to the first $K$ eigenfunctions are invisible at fixed $K$. Under local alternatives $\delta=h/\sqrt n$, the limit is noncentral chi-squared with noncentrality $\frac12\sum_{k\leq K}\langle h,\phi_k\rangle^2/\lambda_k$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 225](../../paper-225-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
