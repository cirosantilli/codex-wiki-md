<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

**Within the 1424 complete records displayed here, employed respondents report more frequent use on average in the ordinal sense of positive pairwise association. The overall [independence](../../../independent-random-variables.md) test is significant, but its sample association magnitude is modest and the result is observational. Some printed ordinal summaries are internally inconsistent.**

Compare row [percentages](../../../percentage.md) because employment groups have different sizes. Never-use is reported by $219/599=36.56\%$ of the non-employed group and $240/825=29.09\%$ of the employed group. Daily use is $24.21\%$ versus $31.39\%$; more-than-daily use is $9.02\%$ versus $13.09\%$. Combining the last two categories gives $33.22\%$ versus $44.48\%$, an employed-minus-non-employed difference of about **11.26 [percentage points](../../../percentage-point.md)**. That threshold comparison is a descriptive summary of the six-category table, not a replacement for the original omnibus test or a newly declared prespecified endpoint. It does not assign equal spacing to the six frequency categories.

Here the row counts, column counts and grand total are additive. Under the [null hypothesis](../../../null-hypothesis.md) of employment–use [independence](../../../independent-random-variables.md), a $2\times6$ [contingency table](../../../contingency-table.md) has $(2-1)(6-1)=5$ [statistical degrees of freedom](../../../statistical-degrees-of-freedom.md). The [Pearson chi-squared statistic](../../../pearson-chi-squared-statistic.md) recomputed from the cells is $21.132241$, agreeing with the printed value, and its [p-value](../../../p-value.md) is about $0.0007648$. The [likelihood-ratio test statistic](../../../likelihood-ratio-test-statistic.md) $G^2\approx21.25379$ gives $p\approx0.000725$. Both reject [independence](../../../independent-random-variables.md) at the conventional 5% and 1% significance levels under the sampling assumptions. The minimum [expected frequency](../../../expected-frequency.md), about $20.61$, gives no sparse-cell warning for this table. The tests compare whole category distributions; they do not by themselves identify one category as the source of the association or establish its causal direction.

[Cramér's V](../../../cramer-s-v.md) is $\sqrt{21.132241/1424}\approx0.12182$. The [generalized phi coefficient](../../../generalized-phi-coefficient.md) coincides with it for this two-row table, while the [contingency coefficient](../../../contingency-coefficient.md) is about $0.121$. These are modest magnitudes; a small [p-value](../../../p-value.md) does not make the relationship large or useful for individual prediction. The employment–use association could change after conditioning on age or other [covariates](../../../covariate.md), and the sample excludes $629$ cases without recorded use. Relative to the employment margins in Figure 1, the omitted complete-case counts are $238$ non-employed and $391$ employed, or about $28.43\%$ and $32.15\%$ of those groups. Different missing fractions alone do not identify the [missing-data mechanism](../../../missing-data-mechanism.md), but they rule out treating complete records as automatically representative of everyone.

The count-based [Goodman and Kruskal's gamma](../../../goodman-and-kruskal-s-gamma.md) is

$$
\gamma=\frac{221614-157488}{221614+157488}\approx0.16915.
$$

With the employment categories ordered non-employed then employed and use ordered from never to more than daily, this positive value means [concordant pairs](../../../concordant-pair.md) outnumber [discordant pairs](../../../discordant-pair.md) among pairs untied on both variables. It is not a 16.9% increase in a person's use and is not a [causal effect](../../../causal-effect.md). Reversing one ordering reverses its sign. Excluding ties can make gamma appreciably larger than tie-adjusted measures.

For use as response and employment as predictor, the cells give [Somers' D](../../../somers-d.md) about $0.12976$, [Kendall's tau-b](../../../kendall-s-tau-b.md) about $0.10362$ and [Stuart's tau-c](../../../stuart-s-tau-c.md) about $0.12650$. The printed Somers value $0.141$ and tau-b $0.108$ should not be presented as verified calculations: the table prints $77297$ second-variable-only ties, whereas its cells give $115073$. The other four pair classes agree with the cells; the printed five classes sum to $975400$, not $\binom{1424}{2}=1013176$. The source does not establish an alternative tie convention that repairs those ordinary identities. The direction remains a weak positive association under either description, but the exact measures require coherent pair counts.

Modal prediction provides another perspective. Without employment information, predicting the globally most frequent use category, never, makes $1424-459=965$ errors. Predicting a separate modal use category in each employment group makes $1424-(219+259)=946$ errors. Thus [Goodman and Kruskal's lambda](../../../goodman-and-kruskal-s-lambda.md) for _use given employment_ is $(965-946)/965\approx0.01969$: about a 1.97% reduction in modal-classification errors. For _employment given use_ the corresponding reduction is $3/599\approx0.00501$. These identify the targets explicitly; the source's row-dependent/column-dependent labels should not be used to reverse the target interpretation. The two small numbers show why an [independence](../../../independent-random-variables.md) test can be significant while coarse modal prediction improves very little. **The supported overall finding is a modest positive association among observed respondents, requiring conditional analysis and a missing-data qualification before broader claims.**

## ↑ Ancestors (10)

1. [4](../4.md)
2. [2020](../../2020-split.md)
3. [Past exam of the digital social research: statistics core course of the University of Oxford](../../split.md)
4. [Digital social research: statistics core course of the University of Oxford](../../../digital-social-research-statistics-core-course-of-the-university-of-oxford.md)
5. [MSc in social science of the internet course of the University of Oxford](../../../msc-in-social-science-of-the-internet-course-of-the-university-of-oxford.md)
6. [Master's course of the University of Oxford](../../../master-s-course-of-the-university-of-oxford.md)
7. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
8. [University of Oxford](../../../university-of-oxford-split.md)
9. [List of universities](../../../list-of-universities.md)
10. [Codex Wiki](../../../split.md)
