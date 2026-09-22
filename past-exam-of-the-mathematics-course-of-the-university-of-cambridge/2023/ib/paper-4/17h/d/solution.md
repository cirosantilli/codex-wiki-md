<h1 id="17h/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Both alternatives have larger $\theta$, so use upper-tail rejection regions. Let $z_{0.95}=\Phi^{-1}(0.95)\simeq1.645$ be the 95th [quantile](../../../../../../quantile-function.md) of the standard [normal distribution](../../../../../../normal-distribution.md).

For the likelihood estimator,

$$
\sum_iY_i\sim\operatorname{Poisson}(\theta S_1).
$$

When $S_1$ is large, the [normal approximation to the Poisson distribution](../../../../../../normal-approximation-to-the-poisson-distribution.md) gives, under $H_0$,

$$
\widehat\theta_{MLE}\approx N\left(1,\frac1{S_1}\right).
$$

An approximate size-$0.05$ test therefore rejects $H_0$ when

$$
\boxed{\widehat\theta_{MLE}
>1+\frac{1.645}{\sqrt{S_1}}}.
$$

When every $x_i$ is large, $Y_i\approx N(\theta x_i,\theta x_i)$ independently. A linear combination of independent normal variables is normal, so under $H_0$,

$$
\widehat\theta_{LS}\approx
N\left(1,\frac{S_3}{S_2^2}\right).
$$

The corresponding approximate size-$0.05$ test rejects when

$$
\boxed{\widehat\theta_{LS}
>1+1.645\frac{\sqrt{S_3}}{S_2}}.
$$

In both cases the null rejection probability is approximately $0.05$, while values near the alternative mean $2$ increasingly fall in the rejection region as the total exposure grows. These are the [normal-approximation tests for a Poisson exposure model](../../../../../../normal-approximation-tests-for-a-poisson-exposure-model.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [17H](../../17h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
