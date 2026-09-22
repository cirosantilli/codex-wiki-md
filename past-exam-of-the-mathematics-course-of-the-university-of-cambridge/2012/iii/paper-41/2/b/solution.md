<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [fixed-effect meta-analysis](../../../../../../fixed-effect-meta-analysis.md) models the studies as estimating a common underlying treatment effect. In a generic inverse-variance version, independent [log odds ratios](../../../../../../log-odds-ratio.md) $y_i$ have approximate distributions $N(\delta,v_i)$ and are pooled with weights $1/v_i$. The supplied [forest plot](../../../../../../forest-plot.md) instead has the [Mantel–Haenszel pooled odds ratio](../../../../../../mantel-haenszel-pooled-odds-ratio.md) weights: for event/nonevent cells $a_i,b_i,c_i,d_i$ and total $n_i$, the normalized weights are proportional to $b_ic_i/n_i$. They reproduce the printed percentages and yield a pooled odds ratio about $2.338$. This is still a common-effect analysis; the two weighting methods should not be silently identified.

A [random-effects meta-analysis](../../../../../../random-effects-meta-analysis.md) allows different true effects: $y_i\mid\delta_i\sim N(\delta_i,v_i)$ with $\delta_i\sim N(\mu,\tau^2)$. The [between-study heterogeneity](../../../../../../between-study-heterogeneity.md) variance $\tau^2$ adds to sampling variance, giving marginal variance $v_i+\tau^2$. Its pooled estimate targets the mean of the study-effect distribution rather than one identical effect. Uncertainty about heterogeneity must also be considered.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 41](../../../paper-41-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
