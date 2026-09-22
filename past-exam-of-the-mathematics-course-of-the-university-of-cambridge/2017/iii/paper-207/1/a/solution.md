<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $y_{WP}$ and $y_{AP}$ for the estimated [log odds ratios](../../../../../../log-odds-ratio.md) relative to the common control. [Indirect treatment comparison](../../../../../../indirect-treatment-comparison.md) uses the consistency relation $\delta_{WA}=\delta_{WP}-\delta_{AP}$. For [independent](../../../../../../independent-random-variables.md) trials, subtraction adds their [variances](../../../../../../variance-split.md), giving

$$
\boxed{\widehat\delta_I=-1.95-(-0.69)=-1.26,\qquad v_I=0.15+0.10=0.25.}
$$

The substantive assumption is [transitivity in network meta-analysis](../../../../../../transitivity-in-network-meta-analysis.md): the study populations, outcome definitions and follow-up are sufficiently comparable, particularly in their distributions of [effect modifiers](../../../../../../effect-modifier.md), that the two control comparisons estimate effects applicable to the same target population. The common control's name alone does not justify that assumption. This also assumes comparable marginal [odds ratios](../../../../../../odds-ratio.md); these need not equal covariate-adjusted [odds ratios](../../../../../../odds-ratio.md) even without [confounding](../../../../../../confounding.md).

Using the supplied rounded [variances](../../../../../../variance-split.md) and the given [standard normal quantile](../../../../../../standard-normal-quantile.md), the approximate [confidence interval](../../../../../../confidence-interval.md) is

$$
\boxed{-1.26\pm2\sqrt{0.25}=(-2.26,-0.26).}
$$

On the [odds ratio](../../../../../../odds-ratio.md) scale this is $e^{-1.26}\simeq0.284$, with approximate limits $(0.104,0.771)$. The estimated odds of recurrent stroke under treatment $W$ are about 28% of those under $A$, a reduction of about 72% in odds. The interval excludes equal odds, so this comparison provides evidence of lower odds under $W$ if the [indirect treatment comparison](../../../../../../indirect-treatment-comparison.md) assumptions hold. These are odds, not a 72% reduction in [probability](../../../../../../probability.md); a [confidence interval](../../../../../../confidence-interval.md) describes the long-run coverage of the procedure, not a [posterior probability](../../../../../../posterior-probability.md) for this particular interval.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
