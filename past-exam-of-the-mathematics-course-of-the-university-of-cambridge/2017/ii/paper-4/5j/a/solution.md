<h1 id="5j/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

**This is the appropriate command for the full [contingency table](../../../../../../contingency-table.md).** It fits a [log-linear model](../../../../../../log-linear-model.md) to the nine cell counts, with [logarithmic link function](../../../../../../logarithmic-link-function.md) and no interaction:

$$
Y_{ij}\sim\operatorname{Poisson}(\mu_{ij}),\qquad\log\mu_{ij}=\alpha+g_i+d_j.
$$

With baseline constraints on $g_i,d_j$, there are five parameters. The factorized means express [independence](../../../../../../independent-random-variables.md) of treatment group and damage category. The [maximum-likelihood estimates](../../../../../../maximum-likelihood-estimator.md) are

$$
\boxed{\widehat\mu_{ij}=\frac{Y_{i+}Y_{+j}}{Y_{++}}=(18,4,8)\quad\text{in each row}.}
$$

Although the experiment fixes each row total at 30, conditioning these independent [Poisson random variables](../../../../../../poisson-distribution.md) on those totals produces the appropriate row-wise [multinomial distribution](../../../../../../multinomial-distribution.md). The [Poisson trick](../../../../../../poisson-trick.md) therefore gives the correct likelihood inference for this [independence log-linear model for a two-way contingency table](../../../../../../independence-log-linear-model-for-a-two-way-contingency-table.md); the margins are nuisance parameters. It tests whether treatment changes the distribution of damage, rather than modelling a binary outcome.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5J](../../5j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
