<h1 id="19h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Any unbiased linear estimator has the form considered in part (b), and its error is the [linear combination of independent normal random variables](../../../../../../linear-combination-of-independent-normal-random-variables.md)

$$
\widetilde\beta-\beta=\sum_i a_i\varepsilon_i
\sim N\left(0,\sigma^2\sum_i a_i^2\right).
$$

The [moment-generating function of a normal distribution](../../../../../../moment-generating-function-of-a-normal-distribution.md) therefore gives, for every nonzero real $\theta$,

$$
\mathbb E_{\beta,\sigma^2}
\left[e^{\theta(\widetilde\beta-\beta)}\right]
=\exp\left(\frac{\theta^2\sigma^2}{2}\sum_i a_i^2\right).
$$

Since the [exponential function](../../../../../../exponential-function.md) is strictly increasing and $\theta^2\sigma^2/2>0$, minimizing this [exponential moment](../../../../../../exponential-moment.md) is exactly the same as minimizing $\sum_i a_i^2$. Part (b) shows that the unique minimizer is $a_i=x_i/S_{xx}$. Thus, independently of the sign or magnitude of $\theta$,

$$
\boxed{\widetilde\beta
=\widehat\beta
=\frac{\sum_i x_iY_i}{\sum_i x_i^2}}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [19H](../../19h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
