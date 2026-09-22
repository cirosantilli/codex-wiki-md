<h1 id="2/2/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

First, the absolute values in the printed limit are an error: the correct [long-run variance of a stationary process](../../../../../../../long-run-variance-of-a-stationary-process.md) is the signed sum of [autocovariances](../../../../../../../autocovariance.md). Directly,

$$
\operatorname{Var}(\overline X_T)=\frac1{T^2}\sum_{s,t=1}^T\gamma_X(t-s),
$$

so

$$
T\operatorname{Var}(\overline X_T)=\sum_{h\in\mathbb Z}\left(1-\frac{|h|}{T}\right)_+\gamma_X(h).
$$

Each coefficient tends to $1$ and has absolute value at most $1$. Absolute summability and the [dominated convergence theorem](../../../../../../../dominated-convergence-theorem.md) therefore give

$$
\boxed{T\operatorname{Var}(\overline X_T)\longrightarrow\sum_{h\in\mathbb Z}\gamma_X(h)=2\pi f_X(0).}
$$

The sum of absolute values is an upper bound, not the general limit. For a concrete counterexample to the printed assertion, take $X_t=\eta_t-\eta_{t-1}$ with unit-[variance](../../../../../../../variance-split.md) iid noise. Then $\gamma(0)=2$, $\gamma(\pm1)=-1$, and other [covariances](../../../../../../../covariance.md) vanish. The absolute sum is $4$, but $\overline X_T=(\eta_T-\eta_0)/T$, so $T\operatorname{Var}(\overline X_T)=2/T\to0$.

For correlated data the [central limit theorem](../../../../../../../central-limit-theorem.md) can still hold under suitable [strong mixing of a stationary process](../../../../../../../strong-mixing-of-a-stationary-process.md) and moment conditions, but the limiting [variance](../../../../../../../variance-split.md) is the [long-run variance of a stationary process](../../../../../../../long-run-variance-of-a-stationary-process.md), rather than the one-observation [variance](../../../../../../../variance-split.md). When it is positive,

$$
\sqrt T(\overline X_T-\mu)\Longrightarrow N\left(0,\sum_h\gamma_X(h)\right).
$$

Positive serial dependence usually increases the [standard error](../../../../../../../standard-error.md), while negative dependence can reduce it. The approximate [effective sample size of a stationary sample](../../../../../../../effective-sample-size-of-a-stationary-sample.md) is $T\gamma_X(0)/\sum_h\gamma_X(h)$ when that denominator is positive. A [long-memory time series](../../../../../../../long-memory-time-series.md) can require a different normalization or a different limit law. Absolute [covariance](../../../../../../../covariance.md) summability alone does not prove a [CLT](../../../../../../../central-limit-theorem.md): if $X_t=V\eta_t$ with a common independent random scale $V$ taking values $1$ and $2$ with equal probabilities and iid $\eta_t$ with the [standard normal distribution](../../../../../../../standard-normal-distribution.md), the off-diagonal [covariances](../../../../../../../covariance.md) are zero, yet $\sqrt T\overline X_T$ has the nonnormal scale-mixture law $V N(0,1)$. The example is not an [ergodic stationary process](../../../../../../../ergodic-stationary-process.md). If the [long-run variance of a stationary process](../../../../../../../long-run-variance-of-a-stationary-process.md) is zero, the usual nondegenerate square-root-$T$ [CLT](../../../../../../../central-limit-theorem.md) is unavailable.

For the causal [AR(1)](../../../../../../../autoregressive-process-of-order-one.md), $|\phi|<1$ and

$$
\boxed{\mu=\frac{m}{1-\phi},\qquad X_t\mid X_{t-1}=x\sim N(m+\phi x,\sigma_\varepsilon^2).}
$$

The [conditional distribution](../../../../../../../conditional-distribution.md) follows because the current innovation is independent of the past.

For a fixed known $\phi$, condition on the observed $X_1$ and use the $n=T-1$ transitions $t=2,\ldots,T$. Their [conditional maximum likelihood](../../../../../../../conditional-maximum-likelihood.md) criterion is, up to constants,

$$
-\frac1{2\sigma_\varepsilon^2}\sum_{t=2}^T\left(X_t-\phi X_{t-1}-(1-\phi)\mu\right)^2.
$$

Differentiating in $\mu$ yields

$$
\boxed{\widehat\mu=\frac{\sum_{t=2}^T(X_t-\phi X_{t-1})}{(T-1)(1-\phi)}.}
$$

Since $X_t-\phi X_{t-1}=(1-\phi)\mu+\varepsilon_t$,

$$
\widehat\mu-\mu=\frac{\sum_{t=2}^T\varepsilon_t}{(T-1)(1-\phi)}.
$$

Thus it is an [unbiased estimator](../../../../../../../unbiased-estimator.md), even conditionally on $X_1$, and

$$
\boxed{\operatorname{Var}(\widehat\mu)=\frac{\sigma_\varepsilon^2}{(T-1)(1-\phi)^2}.}
$$

It has [statistical consistency](../../../../../../../consistency-statistics.md) with [mean-square convergence](../../../../../../../convergence-in-l2.md), and the iid-noise [strong law of large numbers](../../../../../../../strong-law-of-large-numbers.md) also gives almost-sure [statistical consistency](../../../../../../../consistency-statistics.md). Its [conditional distribution](../../../../../../../conditional-distribution.md) is exactly normal with the displayed mean and [variance](../../../../../../../variance-split.md). If $X_0$ is also observed and all $T$ transitions are used, replace $T-1$ by $T$.

The fixed-$\phi$ qualification is necessary for the exact finite-sample claims. If $\phi$ is jointly estimated, conditional [likelihood function](../../../../../../../likelihood-function.md) is [linear regression](../../../../../../../linear-regression-split.md) with an intercept: writing $\bar X_-=n^{-1}\sum_{t=2}^TX_{t-1}$ and $\bar X_+=n^{-1}\sum_{t=2}^TX_t$, the unconstrained estimators are

$$
\widehat\phi=\frac{\sum_{t=2}^T(X_{t-1}-\bar X_-)(X_t-\bar X_+)}{\sum_{t=2}^T(X_{t-1}-\bar X_-)^2},\qquad
\widehat m=\bar X_+-\widehat\phi\bar X_-,\qquad\widehat\mu=\frac{\widehat m}{1-\widehat\phi}.
$$

This ratio is not generally an [unbiased estimator](../../../../../../../unbiased-estimator.md) and does not have the preceding finite-sample [variance](../../../../../../../variance-split.md). Under the usual stationary regression conditions it has [statistical consistency](../../../../../../../consistency-statistics.md); its [asymptotic variance](../../../../../../../asymptotic-variance.md) is $\sigma_\varepsilon^2/(1-\phi)^2$. Indeed, it differs from $\bar X_+$ by $\widehat\phi(X_T-X_1)/(n(1-\widehat\phi))$, an asymptotically negligible endpoint term. Profiling an unknown innovation [variance](../../../../../../../variance-split.md) does not change the fixed-$\phi$ estimate of $\mu$.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [2](../../2.md)
3. [2](../../../2.md)
4. [Paper 208](../../../../paper-208-split.md)
5. [Iii](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
