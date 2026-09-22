<h1 id="19c/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Under the [null hypothesis](../../../../../../null-hypothesis.md), the standardized intercept $Z=\sqrt n(\widehat\alpha-\alpha_0)/\sigma$ is standard normal, and $V=\operatorname{RSS}/\sigma^2$ is independent with [chi-squared distribution](../../../../../../chi-squared-distribution.md) of $\nu=n-2$ degrees of freedom. Consequently the [Student t test for a simple-regression intercept](../../../../../../student-t-test-for-a-simple-regression-intercept.md) uses

$$
\boxed{T=\frac{\widehat\alpha-\alpha_0}{s/\sqrt n}=\frac Z{\sqrt{V/\nu}}\sim t_{n-2}\quad\text{under }H_0.}
$$

Choose a [significance level](../../../../../../significance-level.md) $\gamma\in(0,1)$ before observing the test result. For the two-sided alternative, **reject $H_0$ when $|T|>t_{n-2,\,1-\gamma/2}$**, where the subscript denotes the indicated [quantile](../../../../../../quantile-function.md) of the [Student t-distribution](../../../../../../student-s-t-distribution.md). The null rejection probability is exactly $\gamma$, independent of the nuisance slope and [variance](../../../../../../variance-split.md). Equivalently report the [p-value](../../../../../../p-value.md) $2[1-F_{t_{n-2}}(|T_{\mathrm{obs}}|)]$. The test assumes the normal independent-error model and a positive residual [variance](../../../../../../variance-split.md) estimate. In the intercept-only case with $n>1$, use $s^2=\operatorname{RSS}/(n-1)$ and $t_{n-1}$ instead.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [19C](../../19c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
