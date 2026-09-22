<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the Poisson [variance function](../../../../../../variance-function.md) $V(\mu)=\mu$, the code computes the [Pearson chi-squared statistic](../../../../../../pearson-chi-squared-statistic.md)

$$
X_P^2=\sum_{i=1}^{18}\frac{(Y_i-\widehat\mu_i)^2}{\widehat\mu_i}
$$

and the [Pearson dispersion estimator](../../../../../../pearson-dispersion-estimator.md)

$$
\widehat\phi=\frac{X_P^2}{18-2}=\frac{X_P^2}{16}.
$$

The first quantity measures [goodness of fit](../../../../../../goodness-of-fit.md); the second estimates the [dispersion parameter](../../../../../../dispersion-parameter.md), which equals one in a correctly specified [Poisson regression](../../../../../../poisson-regression.md). A standard rough calculation substitutes the residual deviance for the Pearson statistic and gives

$$
\widehat\phi\simeq\frac{75.806}{16}=4.74.
$$

If the reported upper-tail probability $4.908651\times10^{-11}$ is inverted numerically, the actual Pearson statistic used by the code is about $82.93$, giving $\widehat\phi\simeq5.18$. Either calculation reveals severe [overdispersion](../../../../../../overdispersion.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
