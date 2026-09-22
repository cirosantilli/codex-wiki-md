<h1 id="5j/solution">Solution</h1>

↑ **Parent:** [5J](../5j.md)

A one-parameter [exponential family](../../../../../exponential-family-split.md) with natural statistic $Y$ has density or probability mass function

$$
f_\theta(y)=h(y)\exp\{\theta y-K(\theta)\},
$$

where $\theta$ is the [natural parameter of an exponential family](../../../../../natural-parameter-of-an-exponential-family.md) and $K$ is the [cumulant function of an exponential family](../../../../../cumulant-function-of-an-exponential-family.md). Its [mean parameter](../../../../../mean-parameter-of-an-exponential-family.md) is

$$
\mu(\theta)=K'(\theta).
$$

The [exponential-family deviance](../../../../../exponential-family-deviance.md) from $\theta_1$ to $\theta_2$ is twice the [Kullback-Leibler divergence](../../../../../kullback-leibler-divergence.md):

$$
D(\theta_1,\theta_2)
=2\mathbb E_{\theta_1}
\left[\log\frac{f_{\theta_1}(Y)}{f_{\theta_2}(Y)}\right].
$$

The carrier $h(Y)$ cancels from the likelihood ratio, so, with $\mu_1=\mathbb E_{\theta_1}Y$,

$$
\boxed{
D(\theta_1,\theta_2)
=2\{(\theta_1-\theta_2)\mu_1-K(\theta_1)+K(\theta_2)\}.}
$$

For the [Poisson distribution](../../../../../poisson-distribution.md) with mean $\mu$,

$$
\theta=\log\mu,
\qquad
K(\theta)=e^\theta=\mu.
$$

Therefore

$$
\boxed{
D(\mu_1,\mu_2)
=2\left\{\mu_1\log\frac{\mu_1}{\mu_2}-\mu_1+\mu_2\right\}.}
$$

Writing $\mu_2=\mu_1+\delta$ and applying the [Taylor series](../../../../../taylor-series.md) of $\log(1+\delta/\mu_1)$ gives

$$
D(\mu_1,\mu_1+\delta)
=\frac{\delta^2}{\mu_1}
+O(\delta^3),
$$

so the second-order approximation is

$$
\boxed{D(\mu_1,\mu_2)\simeq
\frac{(\mu_2-\mu_1)^2}{\mu_1}.}
$$

## ↑ Ancestors (10)

1. [5J](../5j.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
