<h1 id="20h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The specified [gamma distribution](../../../../../../gamma-distribution.md) uses shape $k$ and rate $\lambda$. Multiplying its density by the Poisson likelihood gives a posterior density proportional to $\theta^{k+S-1}e^{-(\lambda+n)\theta}$. Thus the [conjugate prior](../../../../../../conjugate-prior.md) calculation gives

$$
\boxed{\theta\mid X_1,\ldots,X_n\sim\Gamma(k+S,\lambda+n).}
$$

For [squared-error loss](../../../../../../squared-error-loss.md), the posterior expected loss is

$$
\mathbb E[(\theta-a)^2\mid X]=\operatorname{Var}(\theta\mid X)
+(a-\mathbb E[\theta\mid X])^2.
$$

It is minimized at the [posterior mean](../../../../../../posterior-mean.md), so the [Bayes estimator](../../../../../../bayes-estimator.md) is

$$
\boxed{\widehat\theta_{\rm B}=\frac{k+S}{\lambda+n}.}
$$

For a fresh conditionally independent Poisson observation, the [posterior predictive probability](../../../../../../posterior-predictive-probability.md) of zero is the posterior expectation of $e^{-\theta}$. Evaluating the gamma integral gives

$$
\boxed{\mathbb P(X_{n+1}=0\mid X_1,\ldots,X_n)
=\left(\frac{\lambda+n}{\lambda+n+1}\right)^{k+S}.}
$$

The samples are independent conditional on $\theta$; integrating out the uncertain common parameter produces the predictive probability above.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [20H](../../20h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
