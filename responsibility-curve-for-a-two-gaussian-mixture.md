# Responsibility curve for a two-Gaussian mixture

↑ **Parent:** [Mixture responsibility](mixture-responsibility.md)

For fixed [statistical parameters](statistical-parameter.md) $\theta$ and $f(x)>0$, [Bayes' theorem](bayes-theorem.md) gives the [mixture responsibility](mixture-responsibility.md)

$$
r_j(x;\theta)=\mathbb P_\theta(Z=j\mid X=x)=\frac{\pi_jf_j(x)}{f(x)}=\mathbb E_\theta[I_j\mid X=x].
$$

It is the [conditional expectation](conditional-expectation.md) of the [mixture allocation indicator](mixture-allocation-indicator.md). This [posterior probability](posterior-probability.md) concerns the hidden label, with $\theta$ held fixed; it does not require a [prior distribution](prior-probability.md) over $\theta$. For a continuous $X$, use the density ratio to define this [conditional distribution](conditional-distribution.md), rather than dividing probabilities of the zero-probability event $X=x$.[Finite Mixtures, section Recovering posterior mixture proportions: Bayes formula for label probabilities conditional on the observation, component parameters, and mixing weights](stan-user-s-guide-by-stan-development-team/finite-mixtures.md)

For the [Two-Gaussian mixture example](two-gaussian-mixture-example.md), the component density ratio is $\phi(x-2)/\phi(x+2)=e^{4x}$, so the [posterior probability](posterior-probability.md) ratio and the [mixture responsibilities](mixture-responsibility.md) are

$$
\frac{r_2(x)}{r_1(x)}=2e^{4x},\qquad r_2(x)=\frac{2e^{4x}}{1+2e^{4x}},\qquad r_1(x)=\frac{1}{1+2e^{4x}}.
$$

At $x=0$ the two unweighted component densities are equal, so the [mixture responsibilities](mixture-responsibility.md) equal the [mixture weights](mixture-weight.md): $r_1(0)=1/3$, $r_2(0)=2/3$. At $x=(\log2)/4$, the second component density is twice the first and its [mixture responsibility](mixture-responsibility.md) is $4/5$. Equal [mixture responsibilities](mixture-responsibility.md) instead occur at $x_*=-(\log2)/4\approx-0.1733$: the more frequent second [mixture component](mixture-component.md) is favored even slightly to the left of the midpoint.

<a id="image-posterior-responsibilities-change-with-x-while-the-stipulated-mixture-weights-stay-fixed"></a>
![](two-gaussian-mixture-posterior-responsibilities.png)

**[Figure 6](#image-posterior-responsibilities-change-with-x-while-the-stipulated-mixture-weights-stay-fixed). Posterior responsibilities change with x while the stipulated mixture weights stay fixed**. Original analytic responsibilities for the same two-Gaussian mixture, with prior label probabilities shown as dotted horizontal lines. Both responsibilities remain strictly between zero and one at every finite x; the vertical marker denotes equal posterior probabilities, not disjoint component supports.

The [mixture weights](mixture-weight.md) describe membership before learning $x$; [mixture responsibilities](mixture-responsibility.md) describe membership after learning $x$. The [law of total expectation](law-of-total-expectation.md) gives $\mathbb E[r_j(X;\theta)]=\pi_j$ under this [statistical model](statistical-model-split.md), although $r_j(x;\theta)$ varies across individual values. In fitting by the [expectation-maximization algorithm](expectation-maximization-algorithm.md), evaluate [mixture responsibilities](mixture-responsibility.md) at the current [statistical parameters](statistical-parameter.md) and recompute them after an update.

## ↑ Ancestors (9)

1. [Mixture responsibility](mixture-responsibility.md)
2. [Finite mixture model](finite-mixture-model.md)
3. [Mixture model](mixture-model.md)
4. [Statistical modelling](statistical-modelling-split.md)
5. [Statistical model](statistical-model-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)
