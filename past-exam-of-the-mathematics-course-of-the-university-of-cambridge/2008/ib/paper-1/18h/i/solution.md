<h1 id="18h/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $\bar X=n^{-1}\sum_iX_i$ and $\bar Y=n^{-1}\sum_iY_i$. Completing the square in each sample, the log [likelihood](../../../../../../likelihood-function.md) is, up to a data-dependent constant,

$$
\ell(\mu_X,\mu_Y)=-\frac n2[(\mu_X-\bar X)^2+(\mu_Y-\bar Y)^2].
$$

The [maximum-likelihood estimators](../../../../../../maximum-likelihood-estimator.md) follow because it is strictly maximized over unrestricted means at $(\bar X,\bar Y)$. Under the null it is maximized at $(\bar X,0)$. Thus the [likelihood ratio](../../../../../../likelihood-ratio.md) is $\Lambda=\exp(-n\bar Y^2/2)$, and the [likelihood-ratio test](../../../../../../likelihood-ratio-test.md) rejects for large $T=-2\log\Lambda=n\bar Y^2$.

Under every null value of $\mu_X$, $Z=\sqrt n\bar Y$ has the standard [Gaussian distribution](../../../../../../normal-distribution.md); hence $T$ has the [chi-squared distribution](../../../../../../chi-squared-distribution.md) with one degree of freedom. Let $z_p=\Phi^{-1}(p)$, where $\Phi$ is the standard Gaussian [cumulative distribution function](../../../../../../cumulative-distribution-function.md). The exact size-$\alpha$ test is

$$
\boxed{\text{reject if }|\sqrt n\bar Y|>z_{1-\alpha/2}.}
$$

The null rejection probability is $2[1-\Phi(z_{1-\alpha/2})]=\alpha$, independently of the nuisance mean $\mu_X$. No randomization is required because the statistic has a continuous distribution.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [18H](../../18h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
