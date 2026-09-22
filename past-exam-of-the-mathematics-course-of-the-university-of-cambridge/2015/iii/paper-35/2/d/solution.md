<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

A [fixed-effect meta-analysis](../../../../../../fixed-effect-meta-analysis.md) assigns [inverse-variance weights](../../../../../../inverse-variance-weight.md). Using the unrounded within-study [variance](../../../../../../variance-split.md) from part (b), this trial has $w=8$, so **its percentage weight is**

$$
\boxed{100\frac8{400}=2\%.}
$$

Using the printed rounded [standard error](../../../../../../standard-error.md) of $0.35$ instead gives approximately $2.04\%$; the raw cell calculation yields the more precise answer.

For a [random-effects meta-analysis](../../../../../../random-effects-meta-analysis.md), the corresponding weight and percentage weight are

$$
\boxed{w^*=\frac1{0.125+\widehat\tau^2},\qquad
100\frac{(0.125+\widehat\tau^2)^{-1}}{\sum_{i=1}^{21}(v_i+\widehat\tau^2)^{-1}}.}
$$

With $\widehat\tau^2=0.05$, its unnormalised weight is $40/7\approx5.714$. The supplied sums of fixed-effect weights do not determine the denominator of the random-effects percentage; the individual $v_i$ are needed. Positive heterogeneity makes the weight distribution more even. Percentage weight measures the trial's contribution to a pooled mean with fixed weights; total influence can also involve re-estimation of heterogeneity.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
