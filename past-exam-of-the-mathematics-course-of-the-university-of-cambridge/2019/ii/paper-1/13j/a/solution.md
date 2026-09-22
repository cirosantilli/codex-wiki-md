<h1 id="13j/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $Y_{ij}$ be the number of ice creams in price category $i\in\{\mathrm{high},\mathrm{low},\mathrm{medium}\}$ and score category $j\in\{\mathrm{excellent},\mathrm{good},\mathrm{poor}\}$. The fitted [Poisson regression](../../../../../../poisson-regression.md) assumes that the nine counts are [independent random variables](../../../../../../independent-random-variables.md) with

$$
Y_{ij}\sim\operatorname{Pois}(\mu_{ij}),
\qquad
\log\mu_{ij}=\alpha_i+\beta_j,
$$

where the [logarithmic link function](../../../../../../logarithmic-link-function.md) is used and excellent is the [reference level in a regression factor](../../../../../../reference-level-in-a-regression-factor.md), so $\beta_{\mathrm{excellent}}=0$. Equivalently,

$$
\mu_{ij}=r_i s_j,
\qquad r_i=e^{\alpha_i},\quad s_j=e^{\beta_j}.
$$

This is the [independence log-linear model for a two-way contingency table](../../../../../../independence-log-linear-model-for-a-two-way-contingency-table.md): price and score have main effects but no interaction.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [13J](../../13j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
