<h1 id="13j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [null hypothesis](../../../../../../null-hypothesis.md) is that price and score are independent, equivalently that the [independence log-linear model for a two-way contingency table](../../../../../../independence-log-linear-model-for-a-two-way-contingency-table.md) is correct. Against the saturated alternative, the reported [Poisson deviance](../../../../../../poisson-deviance.md) is the [likelihood-ratio test statistic](../../../../../../likelihood-ratio-test-statistic.md)

$$
G^2=4.6135.
$$

Under the null and the usual large-sample regularity assumptions, [Wilks theorem](../../../../../../wilks-theorem.md) gives

$$
G^2\xrightarrow{\mathrm d}\chi^2_{(3-1)(3-1)}=\chi^2_4.
$$

The observations must be independent, the cell probabilities must not lie on the boundary of the parameter space, and the expected counts must be large enough for the [chi-squared asymptotic approximation](../../../../../../chi-squared-asymptotic-approximation.md). The fitted counts are either $31/3$ or $28/3$, so the customary expected-count check is comfortably satisfied. Since

$$
4.6135<\chi^2_{4,0.99}\simeq13.277
$$

(equivalently, the [p-value](../../../../../../p-value.md) is about $0.329$), we do not reject the null at the $1\%$ [significance level](../../../../../../significance-level.md). The data provide no significant lack of fit for independence.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [13J](../../13j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
