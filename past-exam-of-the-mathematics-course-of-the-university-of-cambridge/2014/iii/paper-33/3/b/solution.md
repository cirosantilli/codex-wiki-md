<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [generalized linear model](../../../../../../generalized-linear-model.md) specifies independent responses in an [exponential dispersion family](../../../../../../exponential-dispersion-model.md), their means $\mu_i=E(Y_i)$, and a [link function](../../../../../../link-function.md) connecting those means to a [linear predictor](../../../../../../linear-predictor.md). In the common notation,

$$
f_i(y_i)=\exp\left\{\frac{y_i\theta_i-b(\theta_i)}{a_i\phi}+c_i(y_i,a_i\phi)\right\},
\qquad\mu_i=b'(\theta_i),\quad\operatorname{Var}(Y_i)=a_i\phi V(\mu_i),
$$

where $a_i$ are known positive weights, $\phi$ is the common [dispersion parameter](../../../../../../dispersion-parameter.md), and $V(\mu_i)=b''(\theta_i)$ is the [variance function](../../../../../../variance-function.md). The systematic part is

$$
\boxed{g(\mu_i)=x_i^T\beta.}
$$

Here $x_i$ is a row of the known [design matrix](../../../../../../design-matrix.md) and $\beta$ contains the unknown regression coefficients. The [link function](../../../../../../link-function.md) is invertible on the permitted mean domain; the [canonical link function](../../../../../../canonical-link-function.md) takes the mean to the natural parameter. This separates distributional, predictor, and link assumptions: it does not require the response itself to be normally distributed or the mean itself to be linear in the covariates.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
