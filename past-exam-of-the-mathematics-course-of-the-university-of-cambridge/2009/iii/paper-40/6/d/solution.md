<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Both [EM algorithm](../../../../../../expectation-maximization-algorithm.md) and [data augmentation](../../../../../../data-augmentation.md) exploit a latent completion $z$, but they use it differently. EM takes a [conditional expectation](../../../../../../conditional-expectation.md) of the complete-data [log-likelihood](../../../../../../log-likelihood.md) and then maximizes over the parameter, producing a deterministic sequence of point estimates when the M-step is uniquely specified.

In Bayesian [data augmentation](../../../../../../data-augmentation.md), choose a [prior distribution](../../../../../../prior-probability.md) $p(\theta)$ and target

$$
p(\theta,z\mid x)\propto f(x,z;\theta)p(\theta).
$$

Alternate the [Gibbs sampler](../../../../../../gibbs-sampler.md) updates

$$
z^{(t+1)}\sim p(z\mid x,\theta^{(t)}),\qquad\theta^{(t+1)}\sim p(\theta\mid x,z^{(t+1)}).
$$

These are stochastic draws from [full conditional distributions](../../../../../../full-conditional-distribution.md), not an expectation followed by maximization. Their invariant law is the augmented joint [posterior](../../../../../../bayesian-posterior.md), and discarding $z$ gives [posterior](../../../../../../bayesian-posterior.md) inference for $\theta$, including uncertainty rather than only an MLE. A sampled completion followed by maximization would instead be a stochastic EM variant. Individual [likelihood](../../../../../../likelihood-function.md) values along a data-augmentation chain need not increase: the chain is designed to sample a [posterior](../../../../../../bayesian-posterior.md), not to ascend the [likelihood](../../../../../../likelihood-function.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [6](../../6.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
