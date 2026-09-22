<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $S_{xx}=\sum_i x_i^2$, $S_{xy}=\sum_i x_iy_i$, and $\bar y=n^{-1}\sum_i y_i$. The independent observations in the [normal linear model](../../../../../normal-linear-model-split.md) give

$$
L(\alpha,\beta)\propto
\exp\left\{-\frac1{2\sigma^2}\sum_i(y_i-\alpha-\beta x_i)^2\right\}.
$$

The centered design condition $\sum_i x_i=0$ removes the $\alpha\beta$ term:

$$
\sum_i(y_i-\alpha-\beta x_i)^2
=\sum_i y_i^2+n\alpha^2+S_{xx}\beta^2
-2n\bar y\alpha-2S_{xy}\beta.
$$

The stated [prior density](../../../../../prior-density.md) factors into independent [normal distributions](../../../../../normal-distribution.md) for the [regression intercept](../../../../../regression-intercept.md) $\alpha$ and [regression coefficient](../../../../../regression-coefficient.md) $\beta$. Multiplication by the [likelihood function](../../../../../likelihood-function.md) therefore leaves separate quadratic expressions in the two coefficients. Define the positive posterior [variances](../../../../../variance-split.md)

$$
v_\alpha=\left(\frac n{\sigma^2}+\frac1{\tau_0^2}\right)^{-1},\qquad
v_\beta=\left(\frac{S_{xx}}{\sigma^2}+\frac1{\tau_1^2}\right)^{-1},
$$

and the [posterior means](../../../../../posterior-mean.md)

$$
m_\alpha=v_\alpha\left(\frac{n\bar y}{\sigma^2}+\frac{\alpha_0}{\tau_0^2}\right),\qquad
m_\beta=v_\beta\left(\frac{S_{xy}}{\sigma^2}+\frac{\beta_0}{\tau_1^2}\right).
$$

By [completing the square](../../../../../completing-the-square.md), the joint [posterior density](../../../../../posterior-density.md) is

$$
\boxed{\pi(\alpha,\beta\mid\boldsymbol y)
=\frac1{2\pi\sqrt{v_\alpha v_\beta}}
\exp\left\{-\frac{(\alpha-m_\alpha)^2}{2v_\alpha}
-\frac{(\beta-m_\beta)^2}{2v_\beta}\right\}}.
$$

Equivalently,

$$
\boxed{\alpha\mid\boldsymbol y\sim N(m_\alpha,v_\alpha),\qquad
\beta\mid\boldsymbol y\sim N(m_\beta,v_\beta),\qquad
\alpha\perp\beta\mid\boldsymbol y}.
$$

This is [Gaussian conjugacy for a normal linear model](../../../../../gaussian-conjugacy-for-a-normal-linear-model.md). Each posterior [precision parameter](../../../../../precision-parameter.md) is the sum of its data and prior [precision parameters](../../../../../precision-parameter.md). The formulas remain valid when $S_{xx}=0$: all $x_i$ are then zero, so the [posterior distribution](../../../../../bayesian-posterior.md) of $\beta$ equals its [prior distribution](../../../../../prior-probability.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the statistics course of the University of Oxford](../../../../split.md)
6. [Statistics course of the University of Oxford](../../../../../statistics-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
