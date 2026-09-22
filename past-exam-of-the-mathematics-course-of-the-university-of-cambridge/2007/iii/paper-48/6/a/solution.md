<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Both [data augmentation](../../../../../../data-augmentation.md) and the [expectation-maximization algorithm](../../../../../../expectation-maximization-algorithm.md) introduce [latent variables](../../../../../../latent-variable.md) $Z$ that make the complete-data model easier to handle. The observed-data likelihood is obtained by summing or integrating $p(x,z\mid\theta)$ over the missing data, and both methods use the conditional law of $Z$ given the observations and current parameters.

In [data augmentation](../../../../../../data-augmentation.md) for Bayesian inference, one alternates random draws

$$
Z^{(r+1)}\sim p(z\mid x,\theta^{(r)}),\qquad\theta^{(r+1)}\sim p(\theta\mid x,Z^{(r+1)}).
$$

These are [Gibbs sampler](../../../../../../gibbs-sampler.md) updates on the joint [posterior distribution](../../../../../../bayesian-posterior.md); marginal parameter draws explore the whole posterior, including uncertainty, provided the chain converges appropriately. The parameter conditional incorporates its prior.

The [expectation-maximization algorithm](../../../../../../expectation-maximization-algorithm.md) is instead a deterministic optimization procedure. Its E step forms

$$
Q(\theta\mid\theta^{(r)})=\mathbb E_{Z\mid x,\theta^{(r)}}[\log p(x,Z\mid\theta)],
$$

and its M step maximizes this function over $\theta$. Exact steps do not decrease the observed-data [likelihood function](../../../../../../likelihood-function.md). Their aim is a likelihood stationary point, often a local maximum, rather than draws from a parameter distribution. Adding a log prior to the maximization gives a posterior-mode version, which still does not sample the posterior.

**Data augmentation samples conditional missing data and parameters; EM averages the complete-data log likelihood and optimizes parameters.** The E step is an expectation of the log likelihood, not the log of an averaged likelihood, and generally is not equivalent to merely replacing each missing value by its conditional mean. A Monte Carlo E-step approximation is a further variant of EM, not automatically the same procedure as a [data augmentation](../../../../../../data-augmentation.md) chain.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 48](../../../paper-48-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
