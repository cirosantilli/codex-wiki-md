<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Under the usual regular, identifiable, fixed-dimensional setting, the [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md) is an interior point with vanishing [log-likelihood](../../../../../../log-likelihood.md) gradient, and the observed information is positive definite. Define

$$
J=\frac12\nabla^2D(\widehat\theta)=-\nabla^2\log p(y\mid\widehat\theta).
$$

The second-order [Taylor expansion](../../../../../../taylor-expansion.md) of the [Bayesian deviance](../../../../../../bayesian-deviance.md) is

$$
D(\theta)\approx D(\widehat\theta)+(\theta-\widehat\theta)^TJ(\theta-\widehat\theta).
$$

With a [prior density](../../../../../../prior-density.md) approximately constant over the likelihood's concentration region, the [posterior density](../../../../../../posterior-density.md) is therefore proportional to

$$
\exp\{-D(\theta)/2\}\approx\text{constant}\times
\exp\left[-\frac12(\theta-\widehat\theta)^TJ(\theta-\widehat\theta)\right].
$$

Recognizing the [multivariate normal density](../../../../../../multivariate-normal-density.md) gives

$$
\boxed{\theta\mid y\ \dot\sim\ N_p\left(\widehat\theta,\left[\tfrac12\nabla^2D(\widehat\theta)\right]^{-1}\right).}
$$

Typically $J$ grows at rate $n$ and the posterior concentrates in a region of radius $n^{-1/2}$, making higher-order terms negligible under the regularity assumptions. The local flatness assumption concerns this region, not necessarily the entire parameter space. Boundary maxima, unidentified directions, or persistent multiple modes can invalidate this approximation.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
