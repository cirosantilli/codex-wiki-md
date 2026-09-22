<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $\lambda=\sigma^2$, $v=\sigma_0^2$, and $a=\sqrt\rho$. We keep the model's printed coefficient $\sigma^2Z_i$ literally. Its latent [log odds](../../../../../../log-odds.md) can be written

$$
\theta_i=x_i^T\beta+\lambda Z_i+\eta_i,\qquad\eta_i\overset{\mathrm{iid}}\sim N(0,v).
$$

The independence of the $\theta_i$ is conditional on $Z$: they are not marginally independent when the [random effects](../../../../../../random-effect.md) $Z_i$ are correlated.

Holding the other predictors and the random-effect realization fixed, increasing predictor $j$ by one shifts the latent [log odds](../../../../../../log-odds.md) by $\beta_j$, so it multiplies the conditional odds of a late departure by $e^{\beta_j}$. For a binary snow indicator, this compares the snow and no-snow days with other predictors held fixed. This is a conditional [odds ratio](../../../../../../odds-ratio.md), not generally the same as a marginal odds ratio after integrating the random effects.

Randomizing $\theta_i$ allows unmeasured daily conditions to change the success probability beyond the systematic [linear predictor](../../../../../../linear-predictor.md). In this [logistic-normal regression with autoregressive random effects](../../../../../../logistic-normal-regression-with-autoregressive-random-effects.md), let $P_i=\operatorname{logit}^{-1}(\theta_i)$ and $\bar p_i=\mathbb E[P_i]$. The [law of total variance](../../../../../../law-of-total-variance.md) gives

$$
\operatorname{Var}(Y_i)=n_i\bar p_i(1-\bar p_i)+n_i(n_i-1)\operatorname{Var}(P_i),
$$

so the mixture allows [overdispersion](../../../../../../overdispersion.md) beyond a [binomial distribution](../../../../../../binomial-distribution.md) with fixed probability. The correlated part also allows related outcomes on nearby days.

The stationary [autoregressive process of order one](../../../../../../autoregressive-process-of-order-one.md) has $\operatorname{Var}(Z_i)=1$ and $\operatorname{Cov}(Z_i,Z_j)=a^{|i-j|}$. Hence

$$
\boxed{\operatorname{Var}(\theta_i)=\sigma^4+\sigma_0^2,\qquad
\operatorname{Cov}(\theta_i,\theta_j)=\sigma^4\rho^{|i-j|/2}\quad(i\ne j).}
$$

The $\sigma_0^2$ term is unstructured daily variability, whereas $\sigma^4$ is the temporally correlated component under the printed parameterization. Larger $\rho$ gives greater persistence: the lag-$h$ correlation of the latent log odds is $\sigma^4\rho^{h/2}/(\sigma^4+\sigma_0^2)$.

The PDF itself prints both the coefficient $\sigma^2Z_i$ and the requested combination $\sigma^2+\sigma_0^2$. They are inconsistent as a marginal variance. If the intended coefficient were $\sigma Z_i$, the variance and off-diagonal covariance would instead be $\sigma^2+\sigma_0^2$ and $\sigma^2\rho^{|i-j|/2}$. The prior's argument list also repeats $\sigma^2$; its displayed density indicates the intended second variance parameter is $\sigma_0^2$.

There is a further substantive issue with that [improper prior](../../../../../../improper-prior.md). After integrating the latent variables, the observed-data [likelihood function](../../../../../../likelihood-function.md) is positive and continuous at $\lambda=0$ for fixed finite $\beta$, positive $v$, and $\rho\in(0,1)$. On a compact positive-volume set of those parameters it therefore has a positive lower bound for small $\lambda$. The prior density is $1/(\lambda v)$, so integrating over $\lambda$ gives $\int_0^\varepsilon d\lambda/\lambda=\infty$. Thus the stated joint [posterior distribution](../../../../../../bayesian-posterior.md) is improper, an instance of [improper posterior from a log-uniform random-effect scale prior](../../../../../../improper-posterior-from-a-log-uniform-random-effect-scale-prior.md). The requested fixed-parameter conditional laws below are nevertheless proper; their existence does not remedy the joint impropriety.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 216](../../../paper-216-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
