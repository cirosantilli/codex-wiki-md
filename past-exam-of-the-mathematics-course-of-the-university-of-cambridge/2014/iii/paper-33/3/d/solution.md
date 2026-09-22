<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For the gamma [variance function](../../../../../../variance-function.md), the [Pearson dispersion estimator](../../../../../../pearson-dispersion-estimator.md) is

$$
\widehat\phi=\frac1{57}\sum_{i=1}^{61}\frac{(Y_i-\widehat\mu_i)^2}{\widehat\mu_i^2},
$$

using $61-4=57$ [residual degrees of freedom](../../../../../../residual-degrees-of-freedom.md). Under a specified null dispersion $\phi_0$, the scaled statistic based on squared [Pearson residuals](../../../../../../pearson-residual.md) $57\widehat\phi/\phi_0$ has an approximate $\chi^2_{57}$ distribution under the usual residual approximation.

Thus `test1` corresponds to $H_0:\phi=1$, equivalently gamma shape $\alpha=1$, the [exponential distribution](../../../../../../exponential-distribution.md). `test2` corresponds to $H_0:\phi=1/3$, equivalently shape $\alpha=3$. **The null hypotheses concern dispersion or shape, not whether the regression coefficients vanish.**

The code computes lower-tail probabilities. Used as one-sided tests, the alternatives are $\phi<1$ and $\phi<1/3$, respectively, equivalently shapes larger than one and three. At the 5% level the first null is rejected because the lower-tail probability is $1.199504\times10^{-7}$, while the second is not rejected because its probability is $0.3768748$. If the intended alternatives are two-sided, $\phi\ne\phi_0$, these displayed numbers must not be called two-sided [p-values](../../../../../../p-value.md): doubling the smaller tail gives approximately $2.40\times10^{-7}$ and $0.75375$, with the same decisions. The [chi-squared distribution](../../../../../../chi-squared-distribution.md) approximation is not an exact finite-sample gamma identity.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
