<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

[Exchangeability](../../../../../../exchangeable-random-variables.md) means that the joint [prior distribution](../../../../../../prior-probability.md) is invariant under breed relabelling:

$$
p(\theta_1,\ldots,\theta_I)
=p(\theta_{\pi(1)},\ldots,\theta_{\pi(I)})
$$

for every permutation $\pi$. The labels carry no prior information about maximum size. This is reasonable for comparable breeds before observing their measurements when no covariates or biological knowledge distinguish them.

[Exchangeability](../../../../../../exchangeable-random-variables.md) does not imply [independence](../../../../../../independent-random-variables.md). In a [hierarchical Bayesian model](../../../../../../hierarchical-bayesian-model.md), the parameters can be independent conditional on a shared [hyperparameter](../../../../../../hyperparameter.md) but dependent after it is integrated out. Known systematic biological differences would call for a model of those differences, with exchangeability only for the remaining unexplained variation.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
