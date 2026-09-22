<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [null hypothesis](../../../null-hypothesis.md) specifies the population comparison to be tested, for example equality of the population [means](../../../expected-value-split.md) for women and their complement. The [alternative hypothesis](../../../alternative-hypothesis.md) for a [two-sided test](../../../two-sided-hypothesis-test.md) is a nonzero difference. A [Student's t-test](../../../student-s-t-test.md) measures an estimated difference in units of its estimated [standard error](../../../standard-error.md):

$$
t=\frac{\widehat\Delta-0}{\widehat{\operatorname{SE}}(\widehat\Delta)}.
$$

On the reported calibration, the [sampling distribution](../../../sampling-distribution.md) under the [null hypothesis](../../../null-hypothesis.md) is [Student's t-distribution](../../../student-s-t-distribution.md) with $1225$ [statistical degrees of freedom](../../../statistical-degrees-of-freedom.md). Consequently the [two-sided test](../../../two-sided-hypothesis-test.md) has [p-value](../../../p-value.md)

$$
\boxed{p=\Pr\{|T_{1225}|\geq2.5\}\simeq0.01255.}
$$

With this many [statistical degrees of freedom](../../../statistical-degrees-of-freedom.md), the [Student t-distribution](../../../student-s-t-distribution.md) is close to the [standard normal distribution](../../../standard-normal-distribution.md): $|t|=2.5$ exceeds the approximate $5\%$ two-sided critical value $1.96$, but falls short of the $1\%$ value $2.576$. **Using the supplied calibration, reject at the $5\%$ significance level, but not at $1\%$.** The large [statistical degrees of freedom](../../../statistical-degrees-of-freedom.md) justify this comparison; a value $2.5$ need not be significant for an arbitrary very small number of [statistical degrees of freedom](../../../statistical-degrees-of-freedom.md).

The [p-value](../../../p-value.md) is the [probability](../../../probability.md), under the specified [null hypothesis](../../../null-hypothesis.md) and sampling assumptions, of a [test statistic](../../../test-statistic.md) at least as discrepant as the observed one. It is not the [probability](../../../probability.md) that the [null hypothesis](../../../null-hypothesis.md) is true, nor the [probability](../../../probability.md) that the observed difference happened “by chance”. A [significance level](../../../significance-level.md) of $5\%$ controls the long-run [type I error](../../../type-i-and-type-ii-errors.md) rate of the testing procedure when its assumptions hold. Failing to reject at $1\%$ does not prove equality. [Statistical significance](../../../statistical-significance.md) also does not measure the substantive size or importance of a difference.

The reported [sample means](../../../sample-mean.md) place the women's [mean](../../../expected-value-split.md) $1.4$ scale units above the overall [mean](../../../expected-value-split.md). The negative [test statistic](../../../test-statistic.md) can reflect the order of subtraction; it does not reverse that observed ordering. An appropriate pre-specified directional [one-sided test](../../../one-sided-hypothesis-test.md) would have a tail [p-value](../../../p-value.md) approximately $0.00627$ on the supplied calibration, but one cannot choose that direction after inspecting the results simply to halve a [p-value](../../../p-value.md).

There is a design issue behind the numerical calculation: the women are included in the overall sample. [Comparing a subgroup mean with its containing sample mean](../../../comparing-a-subgroup-mean-with-its-containing-sample-mean.md) requires accounting for shared observations. If $w$ is the women's sample fraction and $\overline x_O$ the [mean](../../../expected-value-split.md) for the remaining respondents, then

$$
\overline x=w\overline x_F+(1-w)\overline x_O,\qquad
\overline x_F-\overline x=(1-w)(\overline x_F-\overline x_O).
$$

These two estimates are not [independent](../../../independent-random-variables.md). An ordinary independent-two-sample [Student's t-test](../../../student-s-t-test.md) of women against the entire respondent sample would therefore use an inappropriate [standard error](../../../standard-error.md). The interpretation above accepts the supplied [test statistic](../../../test-statistic.md) and its stated null calibration; a valid analysis of the underlying data should compare disjoint groups, or calculate the shared-sample [covariance](../../../covariance.md) correctly. The summary alone cannot establish which calculation was used. [Simple random sampling](../../../simple-random-sampling.md) supports sampling inference under the stated design, but an observed gender association does not establish a [causal effect](../../../causal-effect.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [2023](../../2023-split.md)
3. [Past exam of the digital social research: statistics core course of the University of Oxford](../../split.md)
4. [Digital social research: statistics core course of the University of Oxford](../../../digital-social-research-statistics-core-course-of-the-university-of-oxford.md)
5. [MSc in social science of the internet course of the University of Oxford](../../../msc-in-social-science-of-the-internet-course-of-the-university-of-oxford.md)
6. [Master's course of the University of Oxford](../../../master-s-course-of-the-university-of-oxford.md)
7. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
8. [University of Oxford](../../../university-of-oxford-split.md)
9. [List of universities](../../../list-of-universities.md)
10. [Codex Wiki](../../../split.md)
