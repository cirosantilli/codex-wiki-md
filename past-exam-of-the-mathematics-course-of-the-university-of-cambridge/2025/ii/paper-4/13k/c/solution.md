<h1 id="13k/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Changing the [reference level in a regression factor](../../../../../../reference-level-in-a-regression-factor.md) from A to B does not change the statistical model, fitted probabilities, likelihood, or deviance. If the first parametrization is

$$
(\beta_0,\beta_B,\beta_C,\beta_M),
$$

then the second is

$$
(\beta'_0,\beta'_A,\beta'_C,\beta'_M)
=(\beta_0+\beta_B,-\beta_B,\beta_C-\beta_B,\beta_M).
$$

Numerically,

$$
\begin{aligned}
1.6855+0.8096&=2.4951,\\
-0.8096&=-0.8096,\\
-0.5423-0.8096&\approx-1.3520,\\
-0.9048&=-0.9048.
\end{aligned}
$$

The A-versus-B test is the same test as the former B-versus-A test, with its sign reversed, so its p-value remains $0.0624$. The malignancy coefficient is unchanged in this additive model, so its p-value remains $0.0175$. The intercept now represents site B rather than site A, so its test changes.

The `siteC` coefficient also changes meaning: in `fit1` it tests C versus A, whereas in `fit2` it tests C versus B. Its standard error and p-value therefore need not agree. The displayed tables show that C versus A is not significant ($p=0.2610$), while C versus B is significant ($p=0.0160$). There is no contradiction: these are different pairwise hypotheses.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [13K](../../13k.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
