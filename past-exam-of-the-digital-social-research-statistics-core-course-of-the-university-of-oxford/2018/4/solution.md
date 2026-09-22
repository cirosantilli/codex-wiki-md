<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

**Age and observed populism classification are associated, but the overall association is small and not a strictly monotone age trend. Populist classification is most common in the 55+ group, about 77.12%, versus 66.77% at ages 18–24; it also falls back to 66.38% at ages 35–44.**

This table has 1692 observations, all respondents with an observed populism classification, because age has no missing values. The within-age Populist percentages are 66.77%, 73.18%, 66.38%, 74.03% and 77.12%, in ascending age-group order. Their Not-populist complements are 33.23%, 26.82%, 33.62%, 25.97% and 22.88%. Comparing the oldest and youngest Populist percentages gives about 10.35 [percentage points](../../../percentage-point.md), but the intermediate reversal prevents describing a uniform rise at every age transition. The row totals 310, 302, 348, 308 and 424 are the classified cases; their differences from the age totals in Figure 1 sum to the 92 missing classifications.

The [Pearson chi-squared test of independence](../../../pearson-chi-squared-test-of-independence.md) gives $X^2\approx15.8680$ on $(5-1)(2-1)=4$ [statistical degrees of freedom](../../../statistical-degrees-of-freedom.md), $p\approx0.003201$. The [likelihood-ratio test](../../../likelihood-ratio-test.md) gives $G^2\approx15.8572$ and $p\approx0.003217$. Both reject [independence](../../../independent-random-variables.md) at 5% and 1% under the usual sampling assumptions. The minimum [expected frequency](../../../expected-frequency.md) is about 85.317, so the large-sample approximation is not threatened by sparse expected counts here. Neither test is specifically a test of a linear or monotone age trend.

The [generalized phi coefficient](../../../generalized-phi-coefficient.md) and [Cramér's V](../../../cramer-s-v.md) are about 0.097, and the [contingency coefficient](../../../contingency-coefficient.md) about 0.096: small unsigned association magnitudes. If the binary classification is coded Not populist before Populist and age groups are ordered younger to older, the ordinal output has a meaningful conventional direction. The 258482 concordant and 205602 discordant pairs give [Goodman and Kruskal's gamma](../../../goodman-and-kruskal-s-gamma.md) about 0.114; [Somers' D](../../../somers-d.md) for classification given age is about 0.046, [Kendall's tau-b](../../../kendall-s-tau-b.md) 0.065 and [Stuart's tau-c](../../../stuart-s-tau-c.md) 0.074. These small positive summaries describe an overall older–Populist tendency while allowing the middle-age reversal. They use different tie or table-size adjustments and are not percentages of respondents caused to change classification by ageing.

[Goodman and Kruskal's lambda](../../../goodman-and-kruskal-s-lambda.md) for predicting classification from age is zero because Populist remains the modal classification in every age row. In the reverse direction, predicting age group from classification improves modal predictions slightly: without classification the most frequent age group has 424 cases, whereas choosing a separate modal age group for each classification yields $117+327=444$ correct predictions. The error reduction is $(444-424)/(1692-424)\approx0.0158$, matching the displayed 0.016. Direction must therefore be stated, rather than treating both lambda numbers as interchangeable. **Age is a relevant control variable for the later comparison, but these cross-sectional associations do not establish an age-related causal mechanism or remove other confounders.**

## ↑ Ancestors (10)

1. [4](../4.md)
2. [2018](../../2018-split.md)
3. [Past exam of the digital social research: statistics core course of the University of Oxford](../../split.md)
4. [Digital social research: statistics core course of the University of Oxford](../../../digital-social-research-statistics-core-course-of-the-university-of-oxford.md)
5. [MSc in social science of the internet course of the University of Oxford](../../../msc-in-social-science-of-the-internet-course-of-the-university-of-oxford.md)
6. [Master's course of the University of Oxford](../../../master-s-course-of-the-university-of-oxford.md)
7. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
8. [University of Oxford](../../../university-of-oxford-split.md)
9. [List of universities](../../../list-of-universities.md)
10. [Codex Wiki](../../../split.md)
