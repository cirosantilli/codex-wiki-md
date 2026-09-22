<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a new independent tumour grown for ten days in B, use $x_0=(1,10,10,0)^T$. Its fitted mean is

$$
\widehat\mu_0=x_0^T\widehat\beta=0.6464+10(15.2174)=152.8204.
$$

Write $h_0=x_0^T(X^TX)^{-1}x_0$. The [prediction interval in a normal linear model](../../../../../../prediction-interval-in-a-normal-linear-model.md) is

$$
\boxed{152.8204\ \pm\ t_{26,\,1-\alpha/2}\,s\sqrt{1+h_0},}
$$

where $s^2=\mathrm{RSS}/26$ and $t_{26,1-\alpha/2}$ is the indicated [Student's t-distribution](../../../../../../student-s-t-distribution.md) [quantile](../../../../../../quantile-function.md). The design information needed to evaluate $h_0$ is not supplied, so a fully numerical interval cannot be recovered from the coefficient [standard errors](../../../../../../standard-error.md) alone: the coefficient covariances are also needed.

To prove coverage, write $Y_0=x_0^T\beta+\varepsilon_0$, with $\varepsilon_0\sim N(0,\sigma^2)$ independent of the original sample. The error $Y_0-x_0^T\widehat\beta$ has a [normal distribution](../../../../../../normal-distribution.md) with mean zero and [variance](../../../../../../variance-split.md) $\sigma^2(1+h_0)$. By the [joint distribution of least-squares and variance estimators](../../../../../../joint-distribution-of-least-squares-and-variance-estimators.md), $26s^2/\sigma^2\sim\chi^2_{26}$ and is independent of $\widehat\beta$; it is also independent of $\varepsilon_0$. Hence the [pivotal quantity](../../../../../../pivotal-quantity.md)

$$
T=\frac{Y_0-x_0^T\widehat\beta}{s\sqrt{1+h_0}}\sim t_{26}.
$$

Consequently $\Pr(-t_{26,1-\alpha/2}\le T\le t_{26,1-\alpha/2})=1-\alpha$, which is exactly the claimed [prediction interval](../../../../../../prediction-interval.md) coverage. This is repeated-sampling coverage conditional on the design, assuming the model; it need not hold conditional on the particular observed training responses. The extra $1$ represents new-observation noise and must not be omitted as in a mean [confidence interval](../../../../../../confidence-interval.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
