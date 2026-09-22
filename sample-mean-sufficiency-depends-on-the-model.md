# Sample mean sufficiency depends on the model

↑ **Parent:** [Sufficient statistic](sufficient-statistic.md)

For the [normal sample sum with known variance](normal-sample-sum-with-known-variance.md), assume [independent and identically distributed](independent-and-identically-distributed-random-variables.md) $X_i\sim N(\mu,\sigma^2)$ with fixed known [variance](variance-split.md) $\sigma^2>0$. The [joint probability density](joint-probability-density.md) factors as

$$
f_\mu(x)=\underbrace{(2\pi\sigma^2)^{-n/2}\exp\left[-\frac{\sum_i x_i^2}{2\sigma^2}\right]}_{h(x)}\underbrace{\exp\left[\frac{\mu\sum_i x_i}{\sigma^2}-\frac{n\mu^2}{2\sigma^2}\right]}_{g_\mu(\sum_i x_i)}.
$$

The [Fisher-Neyman factorization theorem](fisher-neyman-factorization-theorem.md) proves that the sum, and hence the [sample mean](sample-mean.md), is a [sufficient statistic](sufficient-statistic.md) for $\mu$. Its remaining deviations $X_i-\overline X$ have a joint [Gaussian](normal-distribution.md) law independent of $\mu$ and are [independent](independent-random-variables.md) of $\overline X$. If both $\mu$ and $\sigma^2$ are unknown, the [sample mean](sample-mean.md) alone loses information about [variance](variance-split.md); the pair $(\sum_iX_i,\sum_iX_i^2)$ is sufficient for the full [statistical parameter](statistical-parameter.md).

A discrete counterexample shows why a [sample mean](sample-mean.md) is not automatically sufficient for arbitrary [statistical models](statistical-model-split.md). Let $X_1,X_2$ be [independent and identically distributed](independent-and-identically-distributed-random-variables.md) on $\{0,1,2\}$ with

$$
P_\theta(X_i=0)=P_\theta(X_i=2)=\theta/2,\qquad P_\theta(X_i=1)=1-\theta,\qquad 0<\theta<1.
$$

Each observation has [mean](expected-value-split.md) one. The arrangements $(0,2),(1,1),(2,0)$ all give [sample mean](sample-mean.md) one, yet

$$
P_\theta((X_1,X_2)=(1,1)\mid\overline X=1)=\frac{(1-\theta)^2}{(1-\theta)^2+\theta^2/2}.
$$

This conditional [probability](probability.md) is $18/19$ at $\theta=1/4$ and $2/11$ at $\theta=3/4$. The [conditional distribution](conditional-distribution.md) therefore still depends on the unknown [statistical parameter](statistical-parameter.md): this [sample mean](sample-mean.md) is not a [sufficient statistic](sufficient-statistic.md). The useful reduction depends on the family of full-data laws, even when its [mean](expected-value-split.md) stays fixed.

## ↑ Ancestors (5)

1. [Sufficient statistic](sufficient-statistic.md)
2. [Probability and statistics](probability-and-statistics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)
