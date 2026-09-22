<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The most plausible cause is **strong dependence between the [latent variables](../../../../../../latent-variable.md) and [covariance](../../../../../../covariance.md) [hyperparameters](../../../../../../hyperparameter.md) in their joint [posterior distribution](../../../../../../bayesian-posterior.md)**. In the usual conditionally independent [Gaussian process classification](../../../../../../gaussian-process-classification.md) model, put $F=(f(x_1),\ldots,f(x_n))$, $w=\sigma^{-2}$, and $C=w^{-1}R_\tau$. The [probit regression](../../../../../../probit-model.md) likelihood is $\ell(F)=\prod_i\Phi((2y_i-1)F_i)$, while $F\mid w,\tau$ has a [multivariate normal distribution](../../../../../../multivariate-normal-distribution.md) with [covariance matrix](../../../../../../covariance-matrix.md) $C$.

For distinct inputs and positive length scales, $R_\tau$ is positive definite. Its Gaussian [probability density function](../../../../../../probability-density-function.md) contributes

$$
p(F\mid w,\tau)\propto w^{n/2}|R_\tau|^{-1/2}
\exp\!\left(-\frac w2F^\top R_\tau^{-1}F\right).
$$

The unit-rate exponential [prior distribution](../../../../../../prior-probability.md) on $w$ therefore gives

$$
\boxed{w\mid F,\tau,y\sim\operatorname{Gamma}\!\left(1+\frac n2,\ 1+\frac12F^\top R_\tau^{-1}F\right).}
$$

Its scale is tightly tied to the current magnitude and shape of $F$. Changing $\tau$ changes the [eigenvectors](../../../../../../eigenvector.md) and [eigenvalues](../../../../../../eigenvalue.md) of its [covariance matrix](../../../../../../covariance-matrix.md); a latent vector typical under the old [covariance](../../../../../../covariance.md) may be very atypical under a substantially different one. Holding $F$ fixed can thus restrict the range of a hyperparameter update, and holding the hyperparameters fixed restricts the next latent-[function](../../../../../../function-split.md) update. Even exact sampling of each [full conditional distribution](../../../../../../full-conditional-distribution.md) can move slowly along a narrow ridge of the joint [posterior distribution](../../../../../../bayesian-posterior.md).

Binary observations provide limited information about the absolute size of large correctly signed latent values. This can leave substantial scale uncertainty and strengthen the dependence. Long correlation lengths can also make the [covariance matrix](../../../../../../covariance-matrix.md) nearly singular and the latent coordinates highly dependent. These are plausible explanations for a large [mixing time](../../../../../../mixing-time-of-a-markov-chain.md), not proofs that every data set causes slow convergence. A [blocked Gibbs sampler](../../../../../../blocked-gibbs-sampler.md) removes dependence within its chosen blocks, but not dependence between them. Repeated identical inputs should be represented by one shared latent value; otherwise the nominal Gaussian [matrix](../../../../../../matrix.md) is singular and the displayed inverse formula must be replaced by a representation on its support.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 216](../../../paper-216-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
