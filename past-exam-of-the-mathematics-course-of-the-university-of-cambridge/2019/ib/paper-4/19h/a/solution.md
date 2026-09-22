<h1 id="19h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Apart from terms independent of $\beta$, the Gaussian [log-likelihood](../../../../../../log-likelihood.md) is

$$
\ell(\beta,\sigma^2)
=-\frac1{2\sigma^2}\sum_{i=1}^n(Y_i-\beta x_i)^2.
$$

Differentiating with respect to $\beta$ gives

$$
\frac{\partial\ell}{\partial\beta}
=\frac1{\sigma^2}\sum_{i=1}^n x_i(Y_i-\beta x_i).
$$

The unique zero, and hence the [maximum-likelihood estimate](../../../../../../maximum-likelihood-estimation.md), is

$$
\boxed{\widehat\beta=\frac{\sum_i x_iY_i}{\sum_i x_i^2}}.
$$

The same value minimizes the [residual sum of squares](../../../../../../residual-sum-of-squares.md) $\sum_i(Y_i-\beta x_i)^2$, since maximizing the Gaussian likelihood for fixed $\sigma^2$ is equivalent to minimizing this sum. It is therefore also the [least-squares estimator](../../../../../../linear-regression-through-the-origin.md).

## ↑ Ancestors (11)

1. [A](../a.md)
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
