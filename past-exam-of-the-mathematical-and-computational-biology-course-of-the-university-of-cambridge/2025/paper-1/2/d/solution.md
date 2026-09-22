<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Test the [null hypothesis](../../../../../null-hypothesis.md) $H_0:\theta_m=\theta_f=\theta$ against the [alternative hypothesis](../../../../../alternative-hypothesis.md) that the two rate parameters differ. Under $H_0$, the pooled [maximum-likelihood estimate](../../../../../maximum-likelihood-estimator.md) is $\widehat\theta_0=16/36.8\simeq0.434783$. Under the alternative, the estimates are $\widehat\theta_m=8/22\simeq0.363636$ and $\widehat\theta_f=8/14.8\simeq0.540541$.

In the [likelihood-ratio test statistic](../../../../../likelihood-ratio-test-statistic.md), the data-only terms cancel, and both fitted models have total $\widehat\theta S=16$. Consequently,

$$
T=2(\ell_1-\ell_0)
=16\log\frac{\widehat\theta_m\widehat\theta_f}{\widehat\theta_0^2}
=16\log\frac{36.8^2}{4(22)(14.8)}\simeq0.6245.
$$

The [alternative hypothesis](../../../../../alternative-hypothesis.md) adds one parameter, so [Wilks theorem](../../../../../wilks-theorem.md) gives an approximate [chi-squared distribution](../../../../../chi-squared-distribution.md) with one [degree of freedom](../../../../../degree-of-freedom.md). **Do not reject the common-rate model at the 5% level**, since $T<3.841$. The corresponding approximate [p-value](../../../../../p-value.md) is $0.43$. The fitted [expected values](../../../../../expected-value-split.md) are $5.5$ and $3.7$ days, but four observations per group supply little evidence that the underlying [expected values](../../../../../expected-value-split.md) differ; failure to reject does not establish equality. The [chi-squared distribution](../../../../../chi-squared-distribution.md) calibration is asymptotic and should be treated cautiously for these small samples.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../split.md)
6. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
