<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Poisson deviance](../../../../../../poisson-deviance.md) compares the fitted [Poisson regression](../../../../../../poisson-regression.md) with a [saturated statistical model](../../../../../../saturated-statistical-model.md):

$$
D=2\sum_i\left[y_i\log\frac{y_i}{\widehat\mu_i}-(y_i-\widehat\mu_i)\right],
$$

using $0\log0=0$. If the usual [deviance goodness-of-fit test](../../../../../../deviance-goodness-of-fit-test.md) approximation is adequate, compare $27.2$ with a [chi-squared distribution](../../../../../../chi-squared-distribution.md) on $29$ [statistical degrees of freedom](../../../../../../statistical-degrees-of-freedom.md). Its upper-tail [p-value](../../../../../../p-value.md) is about $0.561$, and $D/29=0.938$. **There is no detected lack of fit or evidence of substantial overdispersion from this deviance.** This neither proves the [Poisson regression](../../../../../../poisson-regression.md) correct nor establishes that the slope is nonzero. Small expected counts, dependence or inadequate covariate specification can undermine the reference approximation, so [deviance residuals](../../../../../../deviance-residual.md) and other [regression diagnostics](../../../../../../regression-diagnostics.md) still matter.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 41](../../../paper-41-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
