<h1 id="6/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Under $H_0$, the seven free covariate coefficients all equal zero. The [likelihood-ratio test statistic](../../../../../../../likelihood-ratio-test-statistic.md) is

$$
\boxed{2(\widehat\ell_1-\widehat\ell_0)=462.7531-442.0713=20.6818.}
$$

The larger fit has ten free [statistical parameters](../../../../../../../statistical-parameter.md), compared with three in the constant-rate fit, so the reference [chi-squared distribution](../../../../../../../chi-squared-distribution.md) has **seven [statistical degrees of freedom](../../../../../../../statistical-degrees-of-freedom.md)**. Its 95th percentile is $14.06714$. Therefore reject $H_0$ at 5%; the [p-value](../../../../../../../p-value.md) is approximately $0.0043$, and the covariate model is preferred. The two constrained sex coefficients add no free [statistical parameters](../../../../../../../statistical-parameter.md).

For the dementia-to-death arrow, the [hazard ratio](../../../../../../../hazard-ratio.md) for higher versus lower education is $e^{-1.490}=0.2254$, with approximate 95% [confidence interval](../../../../../../../confidence-interval.md) $(e^{-2.547},e^{-0.4327})=(0.0783,0.6488)$. Thus higher education is associated with a roughly **77.5% lower fitted death [transition intensity](../../../../../../../transition-intensity.md)**, conditional on diagnosis age; the interval excludes one. This is an observational association and is not a direct multiplicative statement about death [probability](../../../../../../../probability.md).

Each additional year of age at diagnosis multiplies the dementia-to-death [transition intensity](../../../../../../../transition-intensity.md) by $e^{0.07984}=1.0831$, with [confidence interval](../../../../../../../confidence-interval.md) $(e^{-0.007765},e^{0.1674})=(0.9923,1.1822)$. The estimate suggests an increase, but the interval includes one, so this individual age coefficient is not significant at 5%. Sex has [hazard ratio](../../../../../../../hazard-ratio.md) one for this transition **by the model's imposed constraint**. The output supplies no estimated sex effect or test of that constraint for this arrow. The nonzero sex coefficient for $1\to2$ must not be mistaken for a sex effect on $2\to3$.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [6](../../../6.md)
4. [Paper 30](../../../../paper-30-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
