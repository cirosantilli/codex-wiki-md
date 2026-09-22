<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

**Among the 1629 complete cases, reported blocking is more common in the populist group: 18.44% versus 11.19%, a difference of about 7.26 [percentage points](../../../percentage-point.md). The full three-category response distributions are associated with classification: $X^2\approx24.9671$, 2 [statistical degrees of freedom](../../../statistical-degrees-of-freedom.md), $p\approx3.79\times10^{-6}$ and [Cramér's V](../../../cramer-s-v.md) about 0.124. This is an association among observed respondents, not a [causal effect](../../../causal-effect.md).**

Read the body percentages within the populism rows. There are 50 Yes responses out of 447 Not-populist respondents and 218 out of 1182 Populist respondents. The corresponding No percentages are 76.73% and 75.38%, while Not know falls from 12.08% to 6.18%. The overall distribution therefore changes in more than just the Yes category. The row-total percentages, 27.44% and 72.56%, describe group composition in the complete-case table, not the conditional blocking rates. Their slight difference from Question 2's 28.25% and 71.75% is consistent with different missing-value patterns.

The [Pearson chi-squared test of independence](../../../pearson-chi-squared-test-of-independence.md) compares the two full response distributions. Under the [null hypothesis](../../../null-hypothesis.md) of [independence](../../../independent-random-variables.md), each cell has [expected frequency](../../../expected-frequency.md) $E_{ij}=n_{i+}n_{+j}/N$, and

$$
X^2=\sum_{i,j}\frac{(O_{ij}-E_{ij})^2}{E_{ij}},\qquad \mathrm{df}=(2-1)(3-1)=2.
$$

The minimum expected count is about 34.849, comfortably above the usual sparse-cell concern. With independent observations and a suitable sampling model, the tiny [p-value](../../../p-value.md) rejects that omnibus null at conventional [significance levels](../../../significance-level.md). The [likelihood-ratio test of independence in a contingency table](../../../likelihood-ratio-test-of-independence-in-a-contingency-table.md) gives $G^2\approx24.6044$, also on 2 [statistical degrees of freedom](../../../statistical-degrees-of-freedom.md), with calculated $p\approx4.54\times10^{-6}$. Its printed 0.000 is a rounded value, not zero.[Details: the product-marginal null, expected counts and asymptotic chi-squared calibration](../../../pearson-s-chi-squared-test-for-count-data-in-the-r-documentation.md)

The [generalized phi coefficient](../../../generalized-phi-coefficient.md) and [Cramér's V](../../../cramer-s-v.md) both equal $\sqrt{X^2/N}\approx0.124$ because the smaller nontrivial table dimension is one. The [contingency coefficient](../../../contingency-coefficient.md) is $\sqrt{X^2/(X^2+N)}\approx0.123$. These are unsigned magnitude measures, not further significance tests or percentages of explained variation. A modest magnitude can be highly significant with a large [sample size](../../../sample-size.md).

The omnibus test does not, by itself, identify which response contrast differs. To target reported Yes specifically, an explicitly derived binary table combines No and Not know as _non-Yes reports_, producing rows $(50,397)$ and $(218,964)$. An uncorrected two-by-two Pearson test gives $X^2\approx12.4292$ on one [statistical degree of freedom](../../../statistical-degrees-of-freedom.md), $p\approx0.000423$. A large-sample [confidence interval](../../../confidence-interval.md) for the difference of reported-Yes proportions is approximately $[0.0359,0.1092]$, or 3.59 to 10.92 [percentage points](../../../percentage-point.md). These are additional count-derived calculations under independent binomial sampling, not values printed in the exam. They address the selected Yes contrast and do not pretend that Not know and No are substantively identical in every respect. As [aggregation can change a contingency-table independence test](../../../aggregation-can-change-a-contingency-table-independence-test.md) explains, the binary and three-category tests have different null hypotheses.

The printed ordinal coefficients, [Goodman and Kruskal's gamma](../../../goodman-and-kruskal-s-gamma.md) 0.295, [Somers' D](../../../somers-d.md) 0.116, [Kendall's tau-b](../../../kendall-s-tau-b.md) 0.117 and [Stuart's tau-c](../../../stuart-s-tau-c.md) 0.093, are arithmetically consistent with the displayed ordering. For example, 134660 concordant and 73239 discordant pairs give $\gamma=(134660-73239)/(134660+73239)\approx0.295$. The full tie counts also partition all $\binom{1629}{2}=1326006$ unordered pairs correctly. However, the three response labels do not establish an ordinal scale. Their arithmetic sign therefore cannot replace the direct Yes comparison or be called the proportion of variation explained. Changing the arbitrary order of Not know and No could change the ordinal summary without changing the nominal association.[GoodmanKruskalGamma and SomersDelta, Details: ordinal-variable requirement and tied-pair treatment](../../../desctools-documentation-for-gamma-somers-d-and-lambda.md)

Both directional values of [Goodman and Kruskal's lambda](../../../goodman-and-kruskal-s-lambda.md) are zero. No is the modal blocking answer in both populism groups, and Populist is the modal classification within each blocking column. Knowing the other variable therefore changes no modal prediction enough to reduce the number of classification errors. This does not contradict the unequal conditional distributions or the chi-squared result. Before generalizing, missing outcomes, missing classifications, the sampling design and possible [confounding](../../../confounding.md) must be considered; a [p-value](../../../p-value.md) does not supply those assumptions.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [2018](../../2018-split.md)
3. [Past exam of the digital social research: statistics core course of the University of Oxford](../../split.md)
4. [Digital social research: statistics core course of the University of Oxford](../../../digital-social-research-statistics-core-course-of-the-university-of-oxford.md)
5. [MSc in social science of the internet course of the University of Oxford](../../../msc-in-social-science-of-the-internet-course-of-the-university-of-oxford.md)
6. [Master's course of the University of Oxford](../../../master-s-course-of-the-university-of-oxford.md)
7. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
8. [University of Oxford](../../../university-of-oxford-split.md)
9. [List of universities](../../../list-of-universities.md)
10. [Codex Wiki](../../../split.md)
