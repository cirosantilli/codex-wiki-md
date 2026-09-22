<h1 id="4/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $e(x)=\mathbb P(A=1\mid X=x)$ and let $\widehat e$ be a consistent estimate. The [inverse-probability-weighted estimator of the average treatment effect](../../../../../../../inverse-probability-weighted-estimator-of-the-average-treatment-effect.md) is

$$
\boxed{
\widehat\tau_{\rm IPW}
=\frac1n\sum_{i=1}^n\left\{
\frac{A_iY_i}{\widehat e(X_i)}-
\frac{(1-A_i)Y_i}{1-\widehat e(X_i)}
\right\}}.
$$

Under the exchangeability, consistency, and positivity conditions in part ii, and consistent estimation of the [propensity score](../../../../../../../propensity-score.md), its probability limit is

$$
\mathbb E[Y(1)]-\mathbb E[Y(0)],
$$

so it consistently estimates the [average treatment effect](../../../../../../../average-treatment-effect.md). It does not require the additive outcome-regression model used to interpret the ordinary-least-squares coefficient.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Paper 221](../../../../paper-221-split.md)
5. [Iii](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
