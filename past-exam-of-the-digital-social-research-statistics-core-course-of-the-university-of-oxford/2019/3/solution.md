<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

**Greater technology distrust is associated with lower efficacy in the overall sample. The omnibus evidence against [independence](../../../independent-random-variables.md) is strong, while the unsigned association magnitude is modest: $X^2\approx107.727$ on 6 [statistical degrees of freedom](../../../statistical-degrees-of-freedom.md), $p\approx6.10\times10^{-21}$ and [Cramér's V](../../../cramer-s-v.md) about 0.148.** The [observational study](../../../observational-study.md) does not establish that changing trust would cause efficacy to change.

Rows identify the technology response and columns identify efficacy. Each body [percentage](../../../percentage.md) is a within-row [conditional probability](../../../conditional-probability.md) estimate, not a column [percentage](../../../percentage.md). For example, $166/336=49.40\%$ of those who strongly disagree with the distrust statement have High efficacy, whereas $199/718=27.72\%$ of those who agree do. The difference is about 21.69 [percentage points](../../../percentage-point.md). High efficacy decreases across all four rows: 49.40%, 42.41%, 31.02%, 27.72%. Low efficacy is 20.54% in the strongly-disagree row, 18.00% in Disagree, 21.43% in Neutral and 34.26% in Agree. Thus the overall pattern is clear without claiming that every category changes monotonically: the low-efficacy proportion initially falls, and the Medium proportion peaks at 47.55% among neutral respondents.

For the [Pearson chi-squared test of independence](../../../pearson-chi-squared-test-of-independence.md), the [null hypothesis](../../../null-hypothesis.md) says that the two categorical variables are [independent](../../../independent-random-variables.md), equivalently that the efficacy distribution is the same in every technology-response row. With row totals $n_{i+}$ and column totals $n_{+j}$, the [expected frequency](../../../expected-frequency.md) under that hypothesis is $E_{ij}=n_{i+}n_{+j}/N$, and

$$
X^2=\sum_{i,j}\frac{(O_{ij}-E_{ij})^2}{E_{ij}},\qquad \mathrm{df}=(4-1)(3-1)=6.
$$

All twelve [expected frequencies](../../../expected-frequency.md) exceed 79, with minimum about 79.844, so sparse expected cells are not the concern here. Under [independent](../../../independent-random-variables.md) sampling and the usual large-sample calibration, the very small [p-value](../../../p-value.md) rejects [independence](../../../independent-random-variables.md) at conventional [significance levels](../../../significance-level.md). This is an omnibus finding: it does not provide a separate adjusted significance test for every pair of row [percentages](../../../percentage.md).[Details: product-marginal null hypothesis and asymptotic chi-squared calibration](../../../pearson-s-chi-squared-test-for-count-data-in-the-r-documentation.md)

The [likelihood-ratio test of independence in a contingency table](../../../likelihood-ratio-test-of-independence-in-a-contingency-table.md) uses $G^2=2\sum_{O_{ij}>0}O_{ij}\log(O_{ij}/E_{ij})$. The supplied $G^2\approx105.146$ with 6 [statistical degrees of freedom](../../../statistical-degrees-of-freedom.md) gives $p\approx2.11\times10^{-20}$. Its displayed 0.000 is rounded, not an exact zero. It corroborates the omnibus finding. The [generalized phi coefficient](../../../generalized-phi-coefficient.md) is $\sqrt{X^2/N}\approx0.209$, the [contingency coefficient](../../../contingency-coefficient.md) is about 0.205, and [Cramér's V](../../../cramer-s-v.md) is $\sqrt{X^2/[N\min(3,2)]}\approx0.148$. These are unsigned measures of association strength rather than three additional significance tests; they do not describe [causal effects](../../../causal-effect.md) or [percentages](../../../percentage.md) of [variance](../../../variance-split.md) explained. Their magnitude and the small [p-value](../../../p-value.md) answer different questions, especially with a large [sample size](../../../sample-size.md).

The ordinal measures use the displayed order: increasing row index means increasing distrust, while increasing column index means decreasing efficacy. There are 882033 [concordant pairs](../../../concordant-pair.md) and 552543 [discordant pairs](../../../discordant-pair.md). Hence [Goodman and Kruskal's gamma](../../../goodman-and-kruskal-s-gamma.md) is

$$
\gamma=\frac{882033-552543}{882033+552543}\approx0.230.
$$

Its positive sign therefore means that increasing distrust tends to accompany movement toward _lower_ efficacy. Under an ascending efficacy order its sign would be negative, by [sign reversal under reversal of one ordinal ordering](../../../sign-reversal-under-reversal-of-one-ordinal-ordering.md). [Goodman and Kruskal's gamma](../../../goodman-and-kruskal-s-gamma.md) ignores tied pairs; it is not a claim that 23% of efficacy variation is explained. The displayed pair counts partition all $\binom{2466}{2}=3039345$ unordered pairs correctly, including ties. [Somers' D](../../../somers-d.md) for efficacy given technology is about 0.151, [Kendall's tau-b](../../../kendall-s-tau-b.md) about 0.158, and [Stuart's tau-c](../../../stuart-s-tau-c.md) about 0.163. Their different denominators handle ties or table dimensions differently, so their differing magnitudes do not constitute disagreement about the direction.[GoodmanKruskalGamma and SomersDelta, Details: tied-pair exclusions and the directional denominator](../../../desctools-documentation-for-gamma-somers-d-and-lambda.md)[KendallTauB and StuartTauC: tie and table-size adjustments](../../../ordinal-association-measures-in-the-desctools-documentation.md)

[Goodman and Kruskal's lambda](../../../goodman-and-kruskal-s-lambda.md) concerns the proportional reduction in errors when predicting a most frequent category, not ordinal movement. Without technology information the modal efficacy category is Medium, producing $2466-972=1494$ errors. Choosing a separate modal efficacy category in each technology row yields $2466-(166+391+233+273)=1403$ errors. Thus $\lambda_{\mathrm{efficacy}\mid\mathrm{technology}}=91/1494\approx0.061$. In the reverse prediction direction the reduction is $80/1544\approx0.052$, matching the other printed lambda. The improvement in modal classification is small even though [independence](../../../independent-random-variables.md) is decisively rejected. Both the conditional [percentages](../../../percentage.md) and these distinct summaries support a real sample association; ethnicity and other possible [confounders](../../../confounder.md) still require attention before any causal account.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [2019](../../2019-split.md)
3. [Past exam of the digital social research: statistics core course of the University of Oxford](../../split.md)
4. [Digital social research: statistics core course of the University of Oxford](../../../digital-social-research-statistics-core-course-of-the-university-of-oxford.md)
5. [MSc in social science of the internet course of the University of Oxford](../../../msc-in-social-science-of-the-internet-course-of-the-university-of-oxford.md)
6. [Master's course of the University of Oxford](../../../master-s-course-of-the-university-of-oxford.md)
7. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
8. [University of Oxford](../../../university-of-oxford-split.md)
9. [List of universities](../../../list-of-universities.md)
10. [Codex Wiki](../../../split.md)
