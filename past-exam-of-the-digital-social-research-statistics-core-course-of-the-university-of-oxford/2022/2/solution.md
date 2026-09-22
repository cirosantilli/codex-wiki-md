<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

These are row percentages, so the comparisons estimate the conditional [probability](../../../probability.md) of recorded [vaccination](../../../vaccination.md) within each NHS trust category. The percentages increase across the ordered trust categories as

$$
41.94\%,\quad55.88\%,\quad62.32\%,\quad88.44\%,\quad91.25\%.
$$

The extreme-category difference is approximately **49.31 [percentage points](../../../percentage-point.md)**, rather than a 49.31% relative increase. The [ordinal categorical variable](../../../ordinal-categorical-variable.md) records an order; the categories do not establish equal numerical trust increments.

Under the [null hypothesis](../../../null-hypothesis.md) of [independence](../../../independent-random-variables.md), the expected count in a cell is its row total times its column total divided by 748. The [Pearson chi-squared statistic](../../../pearson-chi-squared-statistic.md) compares observed and expected counts through

$$
X^2=\sum_{i,j}\frac{(O_{ij}-E_{ij})^2}{E_{ij}}=100.84896.
$$

There are $(5-1)(2-1)=4$ [statistical degrees of freedom](../../../statistical-degrees-of-freedom.md), giving $p\approx6.49\times10^{-21}$. The minimum expected count is approximately 5.015, so the usual expected-count concern is much less acute here than in the income strata. **The table gives strong evidence of a statistical association.** The [likelihood-ratio test of independence in a contingency table](../../../likelihood-ratio-test-of-independence-in-a-contingency-table.md) agrees: its statistic is approximately 81.361 on four [statistical degrees of freedom](../../../statistical-degrees-of-freedom.md), with a very small [p-value](../../../p-value.md). The displayed `0.000` is rounding, not a zero probability.

For magnitude, [Cramér's V](../../../cramer-s-v.md) is

$$
V=\sqrt{100.84896/748}\approx0.3672.
$$

It describes the size of the departure from [independence](../../../independent-random-variables.md) without using the category order or giving a direction. Calling it “moderate” is only a rough contextual description; the actual percentage differences are easier to interpret.

The ordered coefficients describe a positive direction. [Goodman and Kruskal's gamma](../../../goodman-and-kruskal-s-gamma.md) uses only [concordant pairs](../../../concordant-pair.md) and [discordant pairs](../../../discordant-pair.md):

$$
\gamma=\frac{44257-12957}{44257+12957}\approx0.5471.
$$

It excludes [tied pairs](../../../tied-pair-ordinal-data.md), which are frequent when the response has only two categories. It is therefore not a claim that 54.7% of respondents were vaccinated because of their trust. The directional [Somers' D](../../../somers-d.md) for vaccination as response includes pairs tied on that response in its denominator:

$$
D_{Y\mid X}=\frac{44257-12957}{44257+12957+124681}\approx0.1721.
$$

The smaller value reflects the retained ties; it does not contradict the positive [statistical association](../../../statistical-association.md).

The small column-dependent [Goodman and Kruskal's lambda](../../../goodman-and-kruskal-s-lambda.md) has a useful prediction interpretation. Without trust information, always predicting the more frequent vaccinated category gives 121 mistakes. Predicting the majority category separately in each trust row gives $13+15+26+34+28=116$ mistakes. Hence

$$
\lambda_{Y\mid X}=\frac{121-116}{121}=\frac5{121}\approx0.0413.
$$

Trust reduces this particular modal-prediction error by only about 4.13%, despite the strong evidence against [independence](../../../independent-random-variables.md). Most rows retain the same majority category. **Evidence of association, its ordinal direction and improvement in a chosen prediction rule are different questions.** None establishes that changing trust would change an individual's [vaccination status](../../../vaccination-status.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [2022](../../2022-split.md)
3. [Past exam of the digital social research: statistics core course of the University of Oxford](../../split.md)
4. [Digital social research: statistics core course of the University of Oxford](../../../digital-social-research-statistics-core-course-of-the-university-of-oxford.md)
5. [MSc in social science of the internet course of the University of Oxford](../../../msc-in-social-science-of-the-internet-course-of-the-university-of-oxford.md)
6. [Master's course of the University of Oxford](../../../master-s-course-of-the-university-of-oxford.md)
7. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
8. [University of Oxford](../../../university-of-oxford-split.md)
9. [List of universities](../../../list-of-universities.md)
10. [Codex Wiki](../../../split.md)
