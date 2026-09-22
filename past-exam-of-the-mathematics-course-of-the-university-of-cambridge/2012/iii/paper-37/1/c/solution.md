<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In an R formula, `I(...)` protects ordinary arithmetic from the formula operators: the predictor is the numerical variable $z=x-165$, rather than an instruction to remove a formula term. [Predictor centering](../../../../../../predictor-centering.md) leaves fitted values and the height slope unchanged but places the intercept at a meaningful height. It often reduces the correlation between intercept and slope estimates.

With $M_i=\mathbf1_{\{i=2\}}$, [treatment contrasts](../../../../../../treatment-contrast.md) use female as the [reference level in a regression factor](../../../../../../reference-level-in-a-regression-factor.md). The fitted [normal linear model](../../../../../../normal-linear-model.md) is

$$
Y_{ij}=\beta_0+\beta_M M_i+\beta_h(x_{ij}-165)+\varepsilon_{ij},\qquad
\varepsilon_{ij}\overset{\rm independent}{\sim}N(0,\sigma^2).
$$

The estimates and their [standard errors](../../../../../../standard-error.md) are

$$
\begin{array}{c|rr}
\text{coefficient}&\text{estimate}&\text{standard error}\\\hline
\beta_0&58.4711&0.8533\\
\beta_M&4.3294&1.4356\\
\beta_h&0.6211&0.1412
\end{array}
$$

The intercept estimates female mean weight at height 165. At that same height the male fitted mean is $58.4711+4.3294=62.8005$. Holding height fixed, the fitted male mean exceeds the female mean by 4.3294 weight units. Within either sex, one additional height unit increases fitted mean weight by 0.6211 weight units. If height is in centimetres and weight in kilograms, these interpretations use centimetres and kilograms accordingly. A [standard error](../../../../../../standard-error.md) for the male intercept would require the [covariance](../../../../../../covariance.md) between $\widehat\beta_0$ and $\widehat\beta_M$, which is not printed.

**The prediction equation is $\widehat Y=58.4711+4.3294M+0.6211(x-165)$.** Predictions for individual students also have residual uncertainty, estimated by $s=5.710$, beyond uncertainty in the fitted mean.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
