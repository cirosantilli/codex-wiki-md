# Identical-mean EM trap

↑ **Parent:** [Known-variance Gaussian mixture EM example](known-variance-gaussian-mixture-em-example.md)

In the [Known-variance Gaussian mixture EM example](known-variance-gaussian-mixture-em-example.md), initialize both [means](expected-value-split.md) at the same value $m$. The [mixture responsibilities](mixture-responsibility.md) are then $1/2$ for every observation. Each [M-step](em-maximization-step.md) sets both [means](expected-value-split.md) to the sample [mean](expected-value-split.md), zero here; the next [E-step](em-expectation-step.md) again gives $1/2$. Thus $(0,0)$ is a [fixed point](fixed-point.md) with [log-likelihood](log-likelihood.md) $-14.593631199$, despite the better fit found from $(-1,1)$.

One can check the failure without trusting an iteration plot. Separate the [means](expected-value-split.md) as $(-a,a)$ and use the [hyperbolic cosine](hyperbolic-cosine.md) identity:

$$
\ell(-a,a)-\ell(0,0)=-3a^2+\sum_{i=1}^6\log\cosh(ay_i)=\frac{\sum_iy_i^2-6}{2}a^2+O(a^4)=6.08a^2+O(a^4).
$$

The [Taylor expansion](taylor-expansion.md) uses $\sum_iy_i^2=18.16$. Small nonzero separation therefore improves the [log-likelihood](log-likelihood.md), whereas translating both [means](expected-value-split.md) to $m$ changes it by $-3m^2$. This [stationary point](stationary-point.md) has both improving and worsening directions. Identical initialization cannot discover the separation because every observation keeps identical label probabilities. Trying several distinct initial fits and comparing their final [log-likelihoods](log-likelihood.md) is useful, but does not prove global optimality.

Keeping the [variance](variance-split.md) fixed also removes a different pathology. With known $\sigma=1$, every component [probability density function](probability-density-function.md) is at most $(2\pi)^{-1/2}$, so $\ell\leq-3\log(2\pi)$. If separate component [variances](variance-split.md) are allowed to shrink without restriction, one [mixture component](mixture-component.md) can concentrate at an observation while another retains positive density at the other observations, making the [likelihood function](likelihood-function.md) unbounded. The fixed positive [variance](variance-split.md) in this example prevents that collapse; it does not remove initialization traps.

## ↑ Ancestors (9)

1. [Known-variance Gaussian mixture EM example](known-variance-gaussian-mixture-em-example.md)
2. [Expectation-maximization algorithm](expectation-maximization-algorithm.md)
3. [Latent variable](latent-variable-split.md)
4. [Statistical modelling](statistical-modelling-split.md)
5. [Statistical model](statistical-model-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [EM likelihood monotonicity](em-likelihood-monotonicity.md)
