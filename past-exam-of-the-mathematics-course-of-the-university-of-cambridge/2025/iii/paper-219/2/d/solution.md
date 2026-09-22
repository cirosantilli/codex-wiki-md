<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The marginal predictor density is

$$
x_i\sim N(\mu,A),
\qquad A=\tau^2+\sigma_x^2.
$$

[Gaussian conditional expectation](../../../../../../gaussian-conditional-expectation.md) gives

$$
\xi_i\mid x_i\sim N\!\left(
\mu+\kappa(x_i-mu),v\right),
\qquad
\kappa=\frac{\tau^2}{A},
\qquad
v=\frac{\tau^2\sigma_x^2}{A}.
$$

Integrating this conditional distribution through the response model yields

$$
y_i\mid x_i\sim N\!\left(
\alpha+\beta[\mu+\kappa(x_i-mu)],
s^2+\beta^2v\right).
$$

When $\tau\gg\sigma_x$, $\kappa\to1$, $v\to\sigma_x^2$, and $A\sim\tau^2$. Hence

$$
L\simeq L_1(\alpha,\beta,\sigma^2)L_2(\mu,\tau^2),
$$

where

$$
L_1=\prod_i\varphi\!\left(y_i;\alpha+\beta x_i,
\sigma^2+\sigma_y^2+\beta^2\sigma_x^2\right),
\qquad
L_2=\prod_i\varphi(x_i;\mu,\tau^2).
$$

The approximate maximum-likelihood estimators are

$$
\boxed{\widehat\mu=\bar x,
\qquad
\widehat{\tau^2}=\frac1N\sum_i(x_i-\bar x)^2.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
