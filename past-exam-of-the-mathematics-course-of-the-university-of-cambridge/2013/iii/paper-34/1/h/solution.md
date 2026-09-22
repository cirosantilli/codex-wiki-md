<h1 id="1/h/solution">Solution</h1>

↑ **Parent:** [H](../h.md)

Fit two [hierarchical Bayesian models](../../../../../../hierarchical-bayesian-model.md) to the same observations, one with the bounded [uniform distribution](../../../../../../continuous-uniform-distribution.md) sampling density and the other with an [exponential distribution](../../../../../../exponential-distribution.md) density. Specify rate versus mean in the exponential model and assign appropriate, scientifically comparable proper [prior distributions](../../../../../../prior-probability.md); that parameter is no longer a literal maximum size. Obtain [posterior distributions](../../../../../../bayesian-posterior.md), for example by [Markov chain Monte Carlo](../../../../../../markov-chain-monte-carlo.md), and check convergence.

At the same observational level in both models use the [Bayesian deviance](../../../../../../bayesian-deviance.md) $D(\phi)=-2\log p(\mathbf y\mid\phi)$, excluding prior densities. Retain the same likelihood constants and consistently either condition on breed effects or integrate them out. Estimate $\overline D=\mathbb E[D(\phi)\mid\mathbf y]$, evaluate $D(\overline\phi)$ at the [posterior mean](../../../../../../posterior-mean.md), and compute the [effective parameter count in DIC](../../../../../../effective-parameter-count-in-dic.md):

$$
p_D=\overline D-D(\overline\phi),\qquad
\boxed{\operatorname{DIC}=\overline D+p_D
=2\overline D-D(\overline\phi).}
$$

Smaller [DIC](../../../../../../deviance-information-criterion.md) favours the fit–complexity tradeoff. Supplement it with [posterior predictive checks](../../../../../../posterior-predictive-check.md); the uniform model's parameter-dependent support and the hierarchical structure make the criterion a diagnostic rather than an automatic definitive decision.

## ↑ Ancestors (11)

1. [H](../h.md)
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
