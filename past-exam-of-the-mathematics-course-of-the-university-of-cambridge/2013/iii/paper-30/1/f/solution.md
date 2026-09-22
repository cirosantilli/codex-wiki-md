<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

A natural next fit is [quadratic regression](../../../../../../quadratic-regression.md), which remains a [normal linear model](../../../../../../normal-linear-model.md) in its unknown [regression coefficients](../../../../../../regression-coefficient.md):

$$
\boxed{Y_i=\beta_0+\beta_1x_i+\beta_2x_i^2+\varepsilon_i,
\qquad \varepsilon_i\overset{\mathrm{iid}}\sim N(0,\sigma^2).}
$$

The new [design matrix](../../../../../../design-matrix.md) has rows $(1,x_i,x_i^2)$ and must have [matrix rank](../../../../../../matrix-rank.md) three; three distinct predictor values suffice. The curved [regression residual](../../../../../../regression-residual.md) pattern suggests trying a positive quadratic term, but its sign and adequacy should be checked after fitting. Inspect the new [regression residuals](../../../../../../regression-residual.md) to see whether the systematic curvature has disappeared.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [1](../../1.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
