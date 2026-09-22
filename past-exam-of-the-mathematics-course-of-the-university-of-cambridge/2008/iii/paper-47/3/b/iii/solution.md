<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For [Beta sampling by gamma ratios](../../../../../../../beta-sampling-by-gamma-ratios.md), use either preceding [chi-squared distribution](../../../../../../../chi-squared-distribution.md) algorithm to generate independent $S\sim\chi^2_{2\alpha}$ and $T\sim\chi^2_{2\beta}$, and return

$$
\boxed{R=S/(S+T).}
$$

Write $W=S+T$, so $S=WR$ and $T=W(1-R)$. The [Jacobian determinant](../../../../../../../jacobian-determinant.md) is $W$. The joint [probability density function](../../../../../../../probability-density-function.md) after this [change of variables](../../../../../../../change-of-variables-formula.md) factors as

$$
\frac{r^{\alpha-1}(1-r)^{\beta-1}}{B(\alpha,\beta)}
\frac{w^{\alpha+\beta-1}e^{-w/2}}{2^{\alpha+\beta}\Gamma(\alpha+\beta)},
\qquad0<r<1,\quad w>0.
$$

Integrating out $w$ proves the [Beta distribution](../../../../../../../beta-distribution.md) for $R$.

A new method is [Beta sampling by uniform order statistics](../../../../../../../beta-sampling-by-uniform-order-statistics.md). Generate $m=\alpha+\beta-1$ independent uniforms, sort them, and return the $\alpha$th [order statistic](../../../../../../../order-statistic.md). There are $\alpha-1$ uniforms below the selected value and $\beta-1$ above it. Selecting their labels and placing the selected observation in $dr$ gives density

$$
\frac{m!}{(\alpha-1)!(\beta-1)!}r^{\alpha-1}(1-r)^{\beta-1},\qquad0<r<1,
$$

which is the [Beta distribution](../../../../../../../beta-distribution.md) density. The integrality of the shape parameters is what makes this order-statistic construction possible.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 47](../../../../paper-47-split.md)
5. [Iii](../../../../split.md)
6. [2008](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
