<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The additive model gives useful evidence for both predictors. To test for no adjusted sex effect, use $H_0:\beta_M=0$ against $H_1:\beta_M\ne0$. The statistic $T=\widehat\beta_M/\operatorname{se}(\widehat\beta_M)$ has a [Student t-distribution](../../../../../../student-s-t-distribution.md) with 97 [statistical degrees of freedom](../../../../../../statistical-degrees-of-freedom.md) under the [normal linear model](../../../../../../normal-linear-model.md) and the [null hypothesis](../../../../../../null-hypothesis.md). Here $T=3.016$ and $p=0.00327$. Similarly, $H_0:\beta_h=0$ against a nonzero common slope gives $T=4.397\sim t_{97}$ under the [null hypothesis](../../../../../../null-hypothesis.md), with $p=2.81\times10^{-5}$. Thus, at a fixed height males have a higher fitted mean weight, and within sex greater height is associated with greater weight.

The interaction model adds $\delta M(x-165)$. Its female height slope is $0.6696$ and its male height slope is $0.6696-0.0977=0.5719$. Test $H_0:\delta=0$ against $H_1:\delta\ne0$ using $T=-0.344\sim t_{96}$ under the [null hypothesis](../../../../../../null-hypothesis.md), or equivalently $T^2\sim F_{1,96}$. The $p$-value is 0.73139. **The additive model is a reasonable parsimonious choice; the data give no evidence for different height slopes between sexes.** This does not establish exact equality of population slopes. The additive model also has the higher adjusted [coefficient of determination](../../../../../../coefficient-of-determination.md), 0.405 versus 0.3996, and a slightly smaller [residual standard error](../../../../../../residual-standard-error.md).

Ignoring sex gives a height slope of 0.8769, appreciably above the adjusted slope 0.6211. This is [omitted-variable bias](../../../../../../omitted-variable-bias.md) in the descriptive regression: a taller group with a larger intercept makes the pooled height association steeper. Algebraically, with $z=x-165$,

$$
\widehat b_{\rm pooled}=\widehat\beta_h+\widehat\beta_M\frac{\sum(z-\bar z)(M-\bar M)}{\sum(z-\bar z)^2}.
$$

The printed estimates imply a positive height-sex [covariance](../../../../../../covariance.md). Pooled and adjusted slopes therefore describe different comparisons; the difference is not evidence that adding sex changed a physical effect of height. For predictions, retain both sex and height, check [regression diagnostics](../../../../../../regression-diagnostics.md), and assess performance on new students. The [residual standard error](../../../../../../residual-standard-error.md) near 5.7 remains substantial and the [coefficient of determination](../../../../../../coefficient-of-determination.md) near 0.42 does not promise precise individual prediction.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
