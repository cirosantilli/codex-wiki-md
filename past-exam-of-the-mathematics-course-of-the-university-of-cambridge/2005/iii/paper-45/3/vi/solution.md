<h1 id="3/vi/solution">Solution</h1>

↑ **Parent:** [Vi](../vi.md)

The accepted values $\theta^{(1)},\ldots,\theta^{(R)}$ have marginal [posterior density](../../../../../../posterior-density.md)

$$
h(\theta\mid k)=\int f(\theta,t\mid k)\,dt=\frac{\pi(\theta)\ell_k(\theta)}{m_k}.
$$

Estimate this one-dimensional density by a [histogram](../../../../../../histogram.md) or [kernel density estimation](../../../../../../kernel-density-estimation.md) from the simulated values. Where $\pi(\theta)>0$, [likelihood reconstruction from posterior simulation](../../../../../../likelihood-reconstruction-from-posterior-simulation.md) gives

$$
\boxed{\widehat\theta_{\mathrm{ML}}\approx\underset{\theta}{\operatorname{argmax}}\ \frac{\widehat h_R(\theta\mid k)}{\pi(\theta)}.}
$$

Use bins or a sufficiently fine grid, and refine near the maximum. For a [histogram](../../../../../../histogram.md) with bins $I_b$, its [posterior](../../../../../../bayesian-posterior.md) mass divided by [prior](../../../../../../prior-probability.md) mass estimates a prior-weighted average of the [likelihood](../../../../../../likelihood-function.md) in that bin:

$$
\frac{R^{-1}\#\{r:\theta^{(r)}\in I_b\}}{\int_{I_b}\pi(u)\,du}\ \longrightarrow\ \frac{\int_{I_b}\pi(u)\ell_k(u)\,du}{m_k\int_{I_b}\pi(u)\,du}.
$$

Narrowing the bins gives pointwise [likelihood](../../../../../../likelihood-function.md) reconstruction at continuous positive-prior points. A flat proper [prior](../../../../../../prior-probability.md) over the search interval makes the highest posterior-density bin approximately the highest-likelihood bin. With a nonconstant [prior](../../../../../../prior-probability.md), maximizing the [posterior](../../../../../../bayesian-posterior.md) alone gives a [maximum a posteriori estimate](../../../../../../maximum-a-posteriori-estimate.md), generally different from [maximum likelihood estimation](../../../../../../maximum-likelihood-estimation.md). Choose [prior](../../../../../../prior-probability.md) support covering the intended search region and include a possible boundary maximum; for $k=0$, $\ell_0(\theta)=E[e^{-\theta L/2}]$ decreases with $\theta$, so the maximum-likelihood estimate is $0$.

The sampled genealogies provide a second [likelihood](../../../../../../likelihood-function.md) reconstruction when the one-dimensional [prior](../../../../../../prior-probability.md) integral is computable. Put

$$
r_k(t)=\int_0^\infty\pi(u)a_k(u,t)\,du.
$$

Their [posterior density](../../../../../../posterior-density.md) is $q(t)r_k(t)/m_k$. Therefore, for any trial value $\vartheta$,

$$
\frac1R\sum_{r=1}^R\frac{a_k(\vartheta,T^{(r)})}{r_k(T^{(r)})}\ \longrightarrow\ \frac1{m_k}\int q(t)a_k(\vartheta,t)\,dt=\frac{\ell_k(\vartheta)}{m_k}.
$$

This is an [importance sampling](../../../../../../importance-sampling.md) estimate of the [likelihood](../../../../../../likelihood-function.md) curve using the [posterior](../../../../../../bayesian-posterior.md) genealogies. It can be maximized over a grid without estimating a [posterior density](../../../../../../posterior-density.md) in $\theta$, provided $r_k(t)>0$ wherever the target integrand is positive and the weights are numerically usable. The ordinary moment estimate $k/a_n$ is not automatically a maximum-likelihood estimate: it uses only the [mean](../../../../../../expected-value.md) equation, while the [likelihood](../../../../../../likelihood-function.md) integrates the entire random branch-length distribution.

## ↑ Ancestors (11)

1. [Vi](../vi.md)
2. [3](../../3.md)
3. [Paper 45](../../../paper-45-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
