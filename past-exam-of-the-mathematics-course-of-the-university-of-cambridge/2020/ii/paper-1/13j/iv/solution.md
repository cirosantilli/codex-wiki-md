<h1 id="13j/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

A suitable [generalized linear model](../../../../../../generalized-linear-model.md) is a [Gamma regression with logarithmic link](../../../../../../gamma-regression-with-logarithmic-link.md):

$$
Y_i\mid x_i\text{ has a gamma distribution},
\qquad \mathbb E(Y_i\mid x_i)=\mu_i,
\qquad
\operatorname{Var}(Y_i\mid x_i)=\phi\mu_i^2,
$$

with

$$
\log\mu_i
=\beta_0+\beta_K\operatorname{numeric}(\text{Kilometres}_i)
+\beta_{\text{Brand}_i}+\beta_{\text{Bonus}_i}.
$$

The [gamma distribution](../../../../../../gamma-distribution.md) is appropriate for a positive, continuous, right-skewed payment, and its [variance function](../../../../../../variance-function.md) allows the conditional variance to grow like the square of the conditional mean instead of assuming constant variance. The [logarithmic link function](../../../../../../logarithmic-link-function.md) also guarantees positive fitted means and represents covariate effects multiplicatively, which accords with the [Box–Cox transformation](../../../../../../box-cox-transformation.md) evidence for a logarithmic scale.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [13J](../../13j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
