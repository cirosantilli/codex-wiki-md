<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For independent [Poisson distributions](../../../../../../poisson-distribution.md), ignoring the factorial term only when taking likelihood differences,

$$
\ell(\mu)=\sum_i\{y_i\log\mu_i-\mu_i-\log(y_i!)\}.
$$

The saturated likelihood maximizes each mean separately at $\widetilde\mu_i=y_i$, including its limiting value at zero. Therefore the [Poisson deviance](../../../../../../poisson-deviance.md) is

$$
\boxed{D=2\{\ell(\widetilde\mu)-\ell(\widehat\mu)\}
=2\sum_{i=1}^{30}\left[y_i\log\frac{y_i}{\widehat\mu_i}-(y_i-\widehat\mu_i)\right],}
$$

where $0\log(0/\widehat\mu_i)$ is defined to be zero and $\widehat\mu_i=e^{3.24926+0.01898a_i}$. The expression is twice a saturated-model [likelihood ratio](../../../../../../likelihood-ratio.md) difference, not twice a likelihood ratio itself.

With sufficiently large fitted counts and regularity, $D$ is approximately $\chi^2_{30-2}$ under a correctly specified [Poisson regression](../../../../../../poisson-regression.md). Here $D=83.351$ on 28 [residual degrees of freedom](../../../../../../residual-degrees-of-freedom.md), with upper-tail probability $2.0935\times10^{-7}$. **The Poisson model fits poorly on this diagnostic.** Its deviance is nearly three times its [degrees of freedom](../../../../../../degree-of-freedom.md), consistent with [overdispersion](../../../../../../overdispersion.md), although a wrong mean function, dependence, or influential islands could also cause the discrepancy. The smaller [Akaike information criterion](../../../../../../akaike-information-criterion.md) than its competitors does not make this an adequate absolute fit.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
