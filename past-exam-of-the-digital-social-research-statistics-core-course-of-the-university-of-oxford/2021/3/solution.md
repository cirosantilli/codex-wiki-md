<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The displayed percentages use row denominators. The relevant comparison is therefore the [conditional probability](../../../conditional-probability.md) of each response within each recorded gender group, rather than the gender composition within a response category.

For the male group, $364/1042\approx34.93\%$ strongly agree and $286/1042\approx27.45\%$ agree. For the female group, the corresponding percentages are $225/1093\approx20.59\%$ and $243/1093\approx22.23\%$. Combining the two agreement categories gives

$$
\boxed{\widehat p_M=\frac{650}{1042}\approx62.38\%,\quad
\widehat p_F=\frac{468}{1093}\approx42.82\%,\quad
\widehat p_M-\widehat p_F\approx19.56\text{ percentage points}.}
$$

The female group has more neutral responses, $24.25\%$ versus $17.47\%$, and a higher combined disagreement percentage, $32.94\%$ versus $20.15\%$. Thus the observed distributions differ in more than a single cell.

The [Pearson chi-squared test](../../../pearson-s-chi-squared-test.md) assesses the [null hypothesis](../../../null-hypothesis.md) of [independence](../../../independent-random-variables.md) in the complete $2\times5$ [contingency table](../../../contingency-table.md). Under that null, the [expected frequency](../../../expected-frequency.md) in a cell is its row total times its column total divided by 2,135. Recalculation gives

$$
X^2=\sum_{i,j}\frac{(O_{ij}-E_{ij})^2}{E_{ij}}\approx90.56953,\qquad
\nu=(2-1)(5-1)=4.
$$

The reported [p-value](../../../p-value.md), approximately $9.97\times10^{-19}$, gives very strong evidence against [independence](../../../independent-random-variables.md) under the test's sampling assumptions. The minimum [expected frequency](../../../expected-frequency.md) is about $106.88$, so sparse expected cells are not a problem here. The test concerns the full five-category distribution, not just the combined agreement comparison.

[Cramér's V](../../../cramer-s-v.md) summarizes the magnitude without imposing an ordering on the gender labels:

$$
V=\sqrt{\frac{90.56953}{2135\min(2-1,5-1)}}\approx0.206.
$$

The small [p-value](../../../p-value.md) does not imply a nearly deterministic relationship. For example, the column-dependent [Goodman and Kruskal's lambda](../../../goodman-and-kruskal-s-lambda.md) is only about $0.026$: choosing the modal response separately within the two groups reduces prediction errors from 1,546 to 1,506, a relative reduction of $40/1546\approx2.59\%$.

The positive [Goodman and Kruskal's gamma](../../../goodman-and-kruskal-s-gamma.md) must be interpreted using the table's chosen ordering. The agreement categories run toward less willingness, and gender has no intrinsic ordinal direction. A sign attached to an arbitrary group coding cannot replace the substantive comparison of [conditional probabilities](../../../conditional-probability.md).

The [NaN](../../../nan.md) displayed for the likelihood-ratio calculation is not a valid [p-value](../../../p-value.md) and is not evidence of no association. The [Pearson chi-squared statistic](../../../pearson-chi-squared-statistic.md) can be independently recomputed from the positive cell counts. None of these calculations identifies a [causal effect](../../../causal-effect.md); the table has not controlled for income or other possible [confounders](../../../confounder.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [2021](../../2021-split.md)
3. [Past exam of the digital social research: statistics core course of the University of Oxford](../../split.md)
4. [Digital social research: statistics core course of the University of Oxford](../../../digital-social-research-statistics-core-course-of-the-university-of-oxford.md)
5. [MSc in social science of the internet course of the University of Oxford](../../../msc-in-social-science-of-the-internet-course-of-the-university-of-oxford.md)
6. [Master's course of the University of Oxford](../../../master-s-course-of-the-university-of-oxford.md)
7. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
8. [University of Oxford](../../../university-of-oxford-split.md)
9. [List of universities](../../../list-of-universities.md)
10. [Codex Wiki](../../../split.md)
