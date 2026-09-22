<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\eta_i=\alpha+\beta\log(x_i+10)+\gamma x_i$. The [Poisson-lognormal random-effect model](../../../../../../poisson-lognormal-random-effect-model.md) assigns each plate a random intensity $\mu_{ij}=e^{\eta_i+\lambda_{ij}}$. Conditional on that intensity its [Poisson distribution](../../../../../../poisson-distribution.md) has mean and variance both $\mu_{ij}$, but marginalizing over the [normal distribution](../../../../../../normal-distribution.md) of the [random effect](../../../../../../random-effect.md) gives

$$
m_i=\mathbb E[Y_{ij}\mid\alpha,\beta,\gamma,\tau]
=e^{\eta_i+\tau^2/2}.
$$

The [law of total variance](../../../../../../law-of-total-variance.md) yields

$$
\operatorname{Var}(Y_{ij})=\mathbb E[\mu_{ij}]+\operatorname{Var}(\mu_{ij})
=\boxed{m_i+m_i^2(e^{\tau^2}-1)}.
$$

This exceeds the mean whenever $\tau>0$. The independent plate effects supply additional heterogeneity without inducing dependence between plates conditional on the global parameters. Also $e^{\eta_i}$ is the median random intensity, not its marginal mean; the factor $e^{\tau^2/2}$ matters for population predictions.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
