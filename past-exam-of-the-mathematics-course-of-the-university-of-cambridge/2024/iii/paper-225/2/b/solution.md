<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $(\widehat\lambda_k,\widehat\phi_k)$ be the leading eigenpairs of the sample [covariance operator](../../../../../../covariance-operator.md). For fixed $K$ with $\lambda_1>\cdots>\lambda_K>\lambda_{K+1}$ and $\lambda_K>0$, the [FPCA mean test](../../../../../../fpca-mean-test.md) uses

$$
T_{K,n}
=n\sum_{k=1}^K
\frac{\langle\overline X_n,\widehat\phi_k\rangle^2}
{\widehat\lambda_k}.
$$

Under the null, consistency of the empirical eigenpairs and the multivariate central limit theorem imply

$$
T_{K,n}\xrightarrow d\chi_K^2.
$$

The level-$\alpha$ test therefore rejects above the $(1-\alpha)$ quantile of the [chi-squared distribution](../../../../../../chi-squared-distribution.md) with $K$ degrees of freedom.

For a fixed mean $\mu$, if at least one leading coordinate $\langle\mu,\phi_k\rangle$, $k\leq K$, is nonzero, then $T_{K,n}\to\infty$ in probability and the test is consistent. It has only null-level asymptotic power against means orthogonal to the first $K$ principal component functions. Under $\mu_n=n^{-1/2}\delta$, the limit is noncentral chi-squared with noncentrality

$$
\boxed{\sum_{k=1}^K\frac{\langle\delta,\phi_k\rangle^2}{\lambda_k}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 225](../../../paper-225-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
