<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

**The displayed age groups have fairly similar employment proportions, with no coherent [monotone](../../../monotonic-function.md) age trend. The printed test reports no evidence against age–employment [independence](../../../independent-random-variables.md); recomputing from the five visible rows reaches the same qualitative conclusion. Their totals and several auxiliary fields nevertheless do not represent one consistent table.**

Each row [percentage](../../../percentage.md) estimates an employment proportion _within that age group_. For example, $105/182=57.69\%$ of the youngest displayed group are employed. The employed proportions in the next four rows are $61.57\%$, $62.26\%$, $56.69\%$ and $57.23\%$. The largest displayed proportion is in the 45–54 group and the smallest in the 55–64 group, a difference of about $5.57$ [percentage points](../../../percentage-point.md). These are conditional [percentages](../../../percentage.md), not the age distribution of employed people. The sequence rises and then falls; there is no simple increasing or decreasing pattern.

The [null hypothesis](../../../null-hypothesis.md) for a [Pearson chi-squared test of independence](../../../pearson-chi-squared-test-of-independence.md) is that the joint category [probabilities](../../../probability.md) factor into their age and employment marginals. Its [expected frequencies](../../../expected-frequency.md) are $E_{ij}=n_{i+}n_{+j}/n$, and its [test statistic](../../../test-statistic.md) adds the standardized squared count discrepancies, $X^2=\sum_{ij}(O_{ij}-E_{ij})^2/E_{ij}$. For a complete $r\times c$ [contingency table](../../../contingency-table.md) with positive margins, the large-sample reference [chi-squared distribution](../../../chi-squared-distribution.md) has $(r-1)(c-1)$ [statistical degrees of freedom](../../../statistical-degrees-of-freedom.md). [Independent](../../../independent-random-variables.md) observations and an appropriate sampling scheme are essential; adequate [expected counts](../../../expected-frequency.md) make the approximation more plausible.[Details: independence null, asymptotic reference distribution and observed/expected counts](../../../pearson-s-chi-squared-test-for-count-data-in-the-r-documentation.md)

Reading only the printed test block, $X^2=4.83463$, $5$ [statistical degrees of freedom](../../../statistical-degrees-of-freedom.md) and $p\approx0.4364$ are mutually compatible. The printed [likelihood-ratio test](../../../likelihood-ratio-test.md) gives nearly the same [p-value](../../../p-value.md), about $0.435$. At a prechosen 5% [significance level](../../../significance-level.md) neither rejects [independence](../../../independent-random-variables.md). This is a failure to find evidence, not proof of equal employment [probabilities](../../../probability.md) at every age. The printed [Cramér's V](../../../cramer-s-v.md) around $0.049$ suggests a small sample association; the [contingency coefficient](../../../contingency-coefficient.md) around $0.048$ has the same broad message. The [generalized phi coefficient](../../../generalized-phi-coefficient.md) is an unsigned chi-squared magnitude here, not evidence for a positive age trend. A small association magnitude and a large [p-value](../../../p-value.md) answer different questions.

But only a $5\times2$ table is actually visible. Those rows total $1730$, with employment column sums $698$ and $1032$, rather than the printed $2053$ with columns $837$ and $1216$. Computing solely from the five visible rows gives

$$
X^2\approx4.034032,\qquad \nu=4,\qquad p\approx0.40142,\qquad V\approx0.04829.
$$

Its [likelihood-ratio test statistic](../../../likelihood-ratio-test-statistic.md) is about $4.03243$, again with $4$ [statistical degrees of freedom](../../../statistical-degrees-of-freedom.md). The smallest count-based [expected frequency](../../../expected-frequency.md) is about $73.43$, comfortably large for this ordinary approximation, but different from the printed minimum $74.20068$. These figures are a labelled analysis of the _visible subset_, not a repaired full dataset. An unprinted sixth age row might explain some intended metadata, but neither its label nor a uniquely justified reconstruction is supplied. The oldest printed label also conflicts with Figures 1 and 8.

The ordinal measures look for an ordered tendency. [Goodman and Kruskal's gamma](../../../goodman-and-kruskal-s-gamma.md) compares [concordant pairs](../../../concordant-pair.md) with [discordant pairs](../../../discordant-pair.md) among pairs untied on both variables. The printed negative gamma, [Somers' D](../../../somers-d.md), [Kendall's tau-b](../../../kendall-s-tau-b.md) and [Stuart's tau-c](../../../stuart-s-tau-c.md) therefore suggest, at most, a very weak tendency toward lower employment at higher age categories under the specified ordering. Their precise magnitudes are not reliable here. The ordinary [unordered-pair partition for ordinal data](../../../unordered-pair-partition-for-ordinal-data.md) fails for the printed pair counts, even when compared with the printed $2053$ cases. On the five visible rows the respective count-based values are about $-0.0356$, $-0.0172$ for employment conditional on age, $-0.0218$ and $-0.0266$. None gives a substantial [monotone](../../../monotonic-function.md) pattern; a near-zero ordinal measure would not exclude a nonmonotone relationship in general.

[Goodman and Kruskal's lambda](../../../goodman-and-kruskal-s-lambda.md) is zero in both predictive directions on the visible table: knowing age does not improve the number of correct predictions made by always choosing the most common employment category, and knowing employment does not improve modal age-category prediction. Zero modal-prediction improvement does not mean every category distribution is identical. **Both the reported test block and the separately recomputed visible-table test fail to reject [independence](../../../independent-random-variables.md); neither justifies asserting no association, a causal age effect, or a coherent full-sample calculation from the contradictory printout.**

## ↑ Ancestors (10)

1. [3](../3.md)
2. [2020](../../2020-split.md)
3. [Past exam of the digital social research: statistics core course of the University of Oxford](../../split.md)
4. [Digital social research: statistics core course of the University of Oxford](../../../digital-social-research-statistics-core-course-of-the-university-of-oxford.md)
5. [MSc in social science of the internet course of the University of Oxford](../../../msc-in-social-science-of-the-internet-course-of-the-university-of-oxford.md)
6. [Master's course of the University of Oxford](../../../master-s-course-of-the-university-of-oxford.md)
7. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
8. [University of Oxford](../../../university-of-oxford-split.md)
9. [List of universities](../../../list-of-universities.md)
10. [Codex Wiki](../../../split.md)
