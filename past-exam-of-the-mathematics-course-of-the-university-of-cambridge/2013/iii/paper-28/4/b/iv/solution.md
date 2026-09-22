<h1 id="4/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Under [quadratic loss](../../../../../../../squared-error-loss.md), the [Bayes estimator under squared error loss](../../../../../../../bayes-estimator-under-squared-error-loss.md) of the latent mean $\lambda$ is its [posterior mean](../../../../../../../posterior-mean.md). For the [Poisson-uniform posterior mean](../../../../../../../poisson-uniform-posterior-mean.md), the [prior distribution](../../../../../../../prior-probability.md) has density $1/2$ on $(1,3)$ and the one-count [Poisson distribution](../../../../../../../poisson-distribution.md) likelihood is $\lambda e^{-\lambda}$. Consequently the [Bayesian posterior](../../../../../../../bayesian-posterior.md) density is proportional to $\lambda e^{-\lambda}$ on that interval, with normalizing integral $\int_1^3\lambda e^{-\lambda}\,d\lambda$.

By conditional independence, $\mathbb E(X_2\mid\lambda,X_1)=\lambda$, so the [law of total expectation](../../../../../../../law-of-total-expectation.md) makes the posterior predictive [expected value](../../../../../../../expected-value.md) equal to this same [posterior mean](../../../../../../../posterior-mean.md). It is

$$
\mathbb E(\lambda\mid X_1=1)=\frac{\int_1^3\lambda^2e^{-\lambda}\,d\lambda}{\int_1^3\lambda e^{-\lambda}\,d\lambda}.
$$

The required antiderivatives are $-(\lambda+1)e^{-\lambda}$ and $-(\lambda^2+2\lambda+2)e^{-\lambda}$. Evaluating at the two endpoints gives

$$
\boxed{\widehat m_{\rm Bayes}=\frac{5e^{-1}-17e^{-3}}{2e^{-1}-4e^{-3}}
=\frac{5e^2-17}{2e^2-4}\approx1.85054.}
$$

This estimate differs from $13/7$: the [Bühlmann credibility estimate](../../../../../../../buhlmann-credibility-premium.md) is an optimal affine rule, while the [Bayes estimator under squared error loss](../../../../../../../bayes-estimator-under-squared-error-loss.md) optimizes over all rules and uses the truncated uniform prior through its exact [Bayesian posterior](../../../../../../../bayesian-posterior.md).

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Paper 28](../../../../paper-28-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
