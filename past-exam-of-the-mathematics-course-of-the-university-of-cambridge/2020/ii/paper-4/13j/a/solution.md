<h1 id="13j/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [generalized linear model](../../../../../../generalized-linear-model.md) assumes independent responses from one [exponential dispersion family](../../../../../../exponential-dispersion-model.md),

$$
f_i(y_i;\theta_i,\sigma_i^2)
=\exp\!\left\{
\frac{y_i\theta_i-b(\theta_i)}{\sigma_i^2}
+c(y_i,\sigma_i^2)
\right\},
$$

where $\sigma_i^2=a_i\sigma^2$, $\mu_i=\mathbb E[Y_i]=b'(\theta_i)$, and a [link function](../../../../../../link-function.md) relates the mean to the [linear predictor](../../../../../../linear-predictor.md) by $g(\mu)=X\beta$. It follows from normalization of the density after shifting the [natural parameter](../../../../../../natural-parameter-of-an-exponential-family.md) that

$$
\mathbb E[e^{t_iY_i}]
=\exp\!\left\{
\frac{b(\theta_i+\sigma_i^2t_i)-b(\theta_i)}{\sigma_i^2}
\right\}.
$$

Independence therefore gives the joint [moment-generating function](../../../../../../moment-generating-function.md)

$$
\mathbb E[e^{t^TY}]
=\exp\!\left\{
\sum_{i=1}^n
\frac{b(\theta_i+a_i\sigma^2t_i)-b(\theta_i)}{a_i\sigma^2}
\right\},
$$

whenever every shifted natural parameter lies in its natural-parameter domain.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [13J](../../13j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
