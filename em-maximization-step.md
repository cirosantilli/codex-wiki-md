# EM maximization step

↑ **Parent:** [Expectation-maximization algorithm](expectation-maximization-algorithm.md)

Maximize $Q(\theta\mid\theta^{(t)})$ over the permitted [statistical parameters](statistical-parameter.md), with the [E-step](em-expectation-step.md) [conditional distribution](conditional-distribution.md) held fixed.[Section 2, printed p. 6: general maximization step](maximum-likelihood-from-incomplete-data-via-the-em-algorithm-by-arthur-pentland-dempster-and-others.md) A [finite mixture model](finite-mixture-model.md) has

$$
Q(\theta\mid\theta^{(t)})=\sum_{i,j}r_{ij}^{(t)}\bigl(\log\pi_j+\log f_j(y_i;\theta)\bigr).
$$

For [normal distributions](normal-distribution.md) with known common [variance](variance-split.md) $\sigma^2>0$ and fixed positive [mixture weights](mixture-weight.md), only the [means](expected-value-split.md) are fitted. Dropping terms independent of these candidate [means](expected-value-split.md) gives

$$
Q(\mu\mid\theta^{(t)})=C-\frac{1}{2\sigma^2}\sum_{i,j}r_{ij}^{(t)}(y_i-\mu_j)^2,\qquad N_j^{(t)}=\sum_ir_{ij}^{(t)},\qquad \mu_j^{(t+1)}=\frac{\sum_ir_{ij}^{(t)}y_i}{N_j^{(t)}}.
$$

The [derivative](derivative.md) in $\mu_j$ is $\sum_ir_{ij}^{(t)}(y_i-\mu_j)/\sigma^2$, and its second [derivative](derivative.md) is $-N_j^{(t)}/\sigma^2$. Thus a positive weighted count gives a unique maximizing [weighted mean](weighted-arithmetic-mean.md). This is a maximization of the surrogate $Q$; the observed-data [log-likelihood](log-likelihood.md) need not be [concave](concave-function.md). Recompute the [mixture responsibilities](mixture-responsibility.md) after updating the [means](expected-value-split.md). The broader [EM for Gaussian mixtures with a common variance](em-for-gaussian-mixtures-with-a-common-variance.md) also estimates [mixture weights](mixture-weight.md) and the shared [variance](variance-split.md).

## ↑ Ancestors (8)

1. [Expectation-maximization algorithm](expectation-maximization-algorithm.md)
2. [Latent variable](latent-variable-split.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
