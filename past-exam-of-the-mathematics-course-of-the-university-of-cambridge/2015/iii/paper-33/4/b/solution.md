<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [generalized cross-validation](../../../../../../generalized-cross-validation.md) curve reaches its minimum at **$\lambda=5$** among the supplied grid values. This balances improved conditioning against shrinkage bias using an estimate of prediction error, rather than choosing the penalty with the smallest training [residual sum of squares](../../../../../../residual-sum-of-squares.md). Nearby values have similar errors, so the plot does not establish a highly precise optimal penalty.

Reading the PDF table at $\lambda=5$ gives the fitted [regression intercept](../../../../../../regression-intercept.md) and slopes:

$$
\boxed{\widehat\alpha=0.8695819,\quad
\widehat\beta=(0.5363716,\ 0.4143406,\ -0.01248621,\ 0.10434493,\ 0.7284822,\ -0.002794344)^T.}
$$

These table entries are necessary because the TeX stores the table only inside a figure. The [ridge regression](../../../../../../ridge-regression.md) slopes are shrunk relative to the zero-penalty fit; their small nonzero values do not represent variable exclusion.

There is a minor source inconsistency: the prose says the predictors are centered, but the table's intercept varies with $\lambda$. With exactly centered predictor columns and an unpenalized intercept it would remain $\overline Y$. The numbers above faithfully report the printed table, while part (a) gives the centered formula and the general uncentered conversion. The table therefore reflects a different or incompletely described preprocessing convention.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
