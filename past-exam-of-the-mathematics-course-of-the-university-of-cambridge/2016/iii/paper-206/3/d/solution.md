<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use [negative binomial regression](../../../../../../negative-binomial-regression.md) with a logarithmic mean link, for example
```
library(MASS)
species_nb <- glm.nb(nspecies ~ altitude, link = log)
```
In the mean-size parametrization,

$$
\mathbb E Y_i=\mu_i=e^{\beta_0+\beta_aa_i},\qquad
\operatorname{Var}(Y_i)=\mu_i+\frac{\mu_i^2}{\theta},\qquad\theta>0.
$$

The extra parameter allows [overdispersion](../../../../../../overdispersion.md) that grows quadratically with the mean, unlike the proportional variance of [Quasi-Poisson regression](../../../../../../quasi-poisson-regression.md).

**The printed assertion needs qualification: a negative-binomial model with fixed size is a generalized linear model.** For known $\theta$, its probability mass function is

$$
p(y;\mu,\theta)=\frac{\Gamma(y+\theta)}{\Gamma(\theta)y!}
\left(\frac{\theta}{\theta+\mu}\right)^\theta
\left(\frac{\mu}{\theta+\mu}\right)^y.
$$

With natural parameter $\eta_c=\log[\mu/(\theta+\mu)]<0$, it has [exponential family](../../../../../../exponential-family-split.md) form

$$
\log p(y)=y\eta_c-b_\theta(\eta_c)+c_\theta(y),\qquad
b_\theta(\eta_c)=-\theta\log(1-e^{\eta_c}),
$$

with dispersion one. A logarithmic link is permitted even though it is not the [canonical link function](../../../../../../canonical-link-function.md). This is the [fixed-size negative binomial generalized linear model](../../../../../../fixed-size-negative-binomial-generalized-linear-model.md).

What prevents a single ordinary fixed-family GLM fit in `glm.nb` is joint estimation of the unknown size $\theta$: it changes the cumulant, carrier, and [variance function](../../../../../../variance-function.md), rather than merely multiplying a fixed variance function by a scalar dispersion. The routine alternates a GLM fit at fixed $\theta$ with size-parameter likelihood updates. Thus the intended distinction is between that enlarged fitting problem and a single fixed-family GLM, not a claim that negative-binomial regression can never be a GLM. The package documentation explicitly supports both conventions: [https://stat.ethz.ch/R-manual/R-patched/library/MASS/html/glm.nb.html](https://stat.ethz.ch/R-manual/R-patched/library/MASS/html/glm.nb.html) and [https://stat.ethz.ch/R-manual/R-patched/library/MASS/html/negative.binomial.html.](https://stat.ethz.ch/R-manual/R-patched/library/MASS/html/negative.binomial.html.)

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
