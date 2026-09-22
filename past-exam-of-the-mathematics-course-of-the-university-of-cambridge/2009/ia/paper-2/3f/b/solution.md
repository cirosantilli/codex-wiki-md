<h1 id="3f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

If $\rho=0$, the [bivariate normal density](../../../../../../bivariate-normal-distribution.md) in part (a) factorizes as

$$
f(x_1,x_2)=
\frac{e^{-(x_1-\mu_1)^2/(2\sigma_1^2)}}{\sqrt{2\pi}\sigma_1}
\frac{e^{-(x_2-\mu_2)^2/(2\sigma_2^2)}}{\sqrt{2\pi}\sigma_2}
=f_1(x_1)f_2(x_2).
$$

Integrating over any product of measurable sets proves [independence of random variables](../../../../../../independent-random-variables.md). Conversely, independent variables with finite second moments have $\mathbb E[X_1X_2]=\mathbb E[X_1]\mathbb E[X_2]$, so their [covariance](../../../../../../covariance.md) is zero and $\rho=\operatorname{Cov}(X_1,X_2)/(\sigma_1\sigma_2)=0$. This proves [independence of uncorrelated jointly normal variables](../../../../../../independence-of-uncorrelated-jointly-normal-variables.md); zero correlation alone would not imply independence without the joint normal assumption.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3F](../../3f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
