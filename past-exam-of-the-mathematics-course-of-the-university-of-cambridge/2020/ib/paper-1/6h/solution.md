<h1 id="6h/solution">Solution</h1>

↑ **Parent:** [6H](../6h.md)

The likelihood contributes precision $n$ and precision-weighted mean $n\overline X$, while the prior contributes precision $\tau^2$ and precision-weighted mean $\tau^2\theta$. By [normal-normal conjugacy with known observation variance](../../../../../normal-normal-conjugacy-with-known-observation-variance.md), the posterior is

$$
\mu\mid X_1,\ldots,X_n
\sim N\left(
\frac{n\overline X+\tau^2\theta}{n+\tau^2},
\frac1{n+\tau^2}\right).
$$

Thus the posterior mean is

$$
\boxed{\widehat\mu=\frac{n\overline X+\tau^2\theta}{n+\tau^2}}.
$$

When $\theta=0$, its expectation under true parameter $\mu$ is $n\mu/(n+\tau^2)$ and its variance is $n/(n+\tau^2)^2$. Hence its frequentist [mean squared error](../../../../../mean-squared-error.md) is

$$
\boxed{\operatorname{MSE}_\mu(\widehat\mu)
=\frac{n+\tau^4\mu^2}{(n+\tau^2)^2}}.
$$

## ↑ Ancestors (10)

1. [6H](../6h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
