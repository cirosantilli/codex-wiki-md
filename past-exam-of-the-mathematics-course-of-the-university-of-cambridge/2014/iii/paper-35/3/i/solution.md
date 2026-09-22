<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

In a [normal linear model](../../../../../../normal-linear-model.md), attach a [continuous spike-and-slab prior](../../../../../../continuous-spike-and-slab-prior.md) to each [regression coefficient](../../../../../../regression-coefficient.md). With suitably scaled predictors, introduce indicators $\gamma_j\sim\operatorname{Bernoulli}(\pi)$ and set

$$
\beta_j\mid\gamma_j=0\sim N(0,s_{0j}^2),\qquad
\beta_j\mid\gamma_j=1\sim N(0,s_{1j}^2),\quad s_{0j}\ll s_{1j}.
$$

The narrow component describes practically negligible effects; the wide component permits substantial ones. Fit the joint [Bayesian posterior](../../../../../../bayesian-posterior.md) of coefficients, indicators and any unknown residual variance. [Bayesian model averaging](../../../../../../bayesian-model-averaging.md) gives shrinkage toward zero for poorly supported effects, while $\mathbb P(\gamma_j=1\mid\mathcal D)$ quantifies wide-component support. A shared [Beta distribution](../../../../../../beta-distribution.md) prior on $\pi$ can represent uncertainty about how many effects are substantial.

**Select on scientifically meaningful effect size**, for example a high $\mathbb P(|\beta_j|>\delta_j\mid\mathcal D)$ for a prechosen threshold in meaningful predictor units. Membership in the wide component alone does not imply a large realized effect: its [normal distribution](../../../../../../normal-distribution.md) still permits values near zero. Correlated predictors also require interpretation of the joint [Bayesian posterior](../../../../../../bayesian-posterior.md), rather than treating each coefficient as an isolated test.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
