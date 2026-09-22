<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Each row of the [contingency table](../../../contingency-table.md) is a [conditional distribution](../../../conditional-distribution.md) of the safety category among respondents with that experience status. Thus the relevant comparison uses row [percentages](../../../percentage.md), rather than interpreting the larger number of respondents with some bad experiences as itself an effect on safety.

The [sample proportions](../../../sample-proportion.md) reporting feeling very safe are $39.59\%$ without bad experiences and $32.78\%$ with some bad experiences: the latter is lower by about $6.81$ [percentage points](../../../percentage-point.md). Feeling fairly safe rises from $28.49\%$ to $34.63\%$, a difference of about $6.14$ [percentage points](../../../percentage-point.md). Feeling unsafe changes only from $31.92\%$ to $32.59\%$, about $0.67$ [percentage points](../../../percentage-point.md). The main descriptive shift is therefore from **very safe toward fairly safe**, rather than a large increase in the unsafe category.

[Pearson's chi-squared test](../../../pearson-s-chi-squared-test.md) tests the [null hypothesis](../../../null-hypothesis.md) that experience status and safety category are [independent](../../../independent-random-variables.md). If that were true, the expected cell count would be its row total times column total divided by $n$. The [Pearson chi-squared statistic](../../../pearson-chi-squared-statistic.md) sums squared observed-minus-expected count differences divided by their expected counts. Here

$$
\boxed{X^2=10.84662,\qquad \mathrm{df}=(2-1)(3-1)=2,\qquad p=0.004412523.}
$$

The expected counts are comfortably large, with minimum approximately $234.7$, so the ordinary large-sample [chi-squared distribution](../../../chi-squared-distribution.md) approximation is appropriate under the sampling assumptions. There is evidence against [independence](../../../independent-random-variables.md) even at the $1\%$ [significance level](../../../significance-level.md). The reported likelihood-ratio result gives the same conclusion.

Magnitude is a separate question. [Cramér's V](../../../cramer-s-v.md) gives

$$
V=\sqrt{\frac{10.84662}{1807}}\simeq0.07748,
$$

which describes a weak [statistical association](../../../statistical-association.md). It does not [mean](../../../expected-value-split.md) that $7.7\%$ of safety is explained. Nor does the [p-value](../../../p-value.md) measure the size of that association.

For ordinal direction, order the experience categories as none, some, and the safety categories from very safe toward unsafe. [Goodman and Kruskal's gamma](../../../goodman-and-kruskal-s-gamma.md) compares [concordant pairs](../../../concordant-pair.md) with [discordant pairs](../../../discordant-pair.md) after excluding tied pairs:

$$
\gamma=\frac{282244-242582}{282244+242582}\simeq0.07557.
$$

Its small positive sign then corresponds to a weak tendency toward less safety among respondents with bad experiences. The sign would reverse if exactly one category ordering were reversed. Because this [contingency table](../../../contingency-table.md) has many ties, the response-direction [Somers' D](../../../somers-d.md), which retains response ties among pairs with different predictor values, is smaller:

$$
D_{Y\mid X}=\frac{39662}{524826+261384}\simeq0.05045.
$$

These coefficients describe ordered association; the omnibus [Pearson's chi-squared test](../../../pearson-s-chi-squared-test.md) tests any departure from [independence](../../../independent-random-variables.md) and does not supply a separate [p-value](../../../p-value.md) for gamma.

The column-dependent [Goodman and Kruskal's lambda](../../../goodman-and-kruskal-s-lambda.md) makes the weak predictive improvement tangible. Predicting the overall most frequent safety category makes $1165$ errors in this table. Using a separate most frequent category within each experience row makes $1145$, giving $\lambda=20/1165\simeq0.0172$, only about a $1.7\%$ reduction in those classification errors.

**The sample supports a statistically detectable but weak association, chiefly a reduced [sample proportion](../../../sample-proportion.md) feeling very safe.** This [observational study](../../../observational-study.md) does not establish that bad experiences cause the change: reverse direction, reporting differences or [confounding](../../../confounding.md) could also contribute. The numerical [p-value](../../../p-value.md) also presumes the sampling and complete-case assumptions appropriate to the observations used.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [2023](../../2023-split.md)
3. [Past exam of the digital social research: statistics core course of the University of Oxford](../../split.md)
4. [Digital social research: statistics core course of the University of Oxford](../../../digital-social-research-statistics-core-course-of-the-university-of-oxford.md)
5. [MSc in social science of the internet course of the University of Oxford](../../../msc-in-social-science-of-the-internet-course-of-the-university-of-oxford.md)
6. [Master's course of the University of Oxford](../../../master-s-course-of-the-university-of-oxford.md)
7. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
8. [University of Oxford](../../../university-of-oxford-split.md)
9. [List of universities](../../../list-of-universities.md)
10. [Codex Wiki](../../../split.md)
