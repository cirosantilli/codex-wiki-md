<h1 id="5i/solution">Solution</h1>

↑ **Parent:** [5I](../5i.md)

In a [generalized linear model](../../../../../generalized-linear-model.md), the [linear predictor](../../../../../linear-predictor.md) is $\eta_i=x_i^T\beta$, a linear combination of the covariates with unknown coefficients. The [link function](../../../../../link-function.md) relates this predictor to the [mean](../../../../../expected-value.md): $g(\mu_i)=\eta_i$. The [canonical link function](../../../../../canonical-link-function.md) chooses the natural parameter of the [exponential family](../../../../../exponential-family-split.md), namely $g(\mu)=\theta(\mu)$. Differentiating the normalization of the density shows that $\mu=K'(\theta)$, so the [canonical link function](../../../../../canonical-link-function.md) is $(K')^{-1}$ on the admissible parameter interval.

For a [Bernoulli distribution](../../../../../bernoulli-distribution.md), the probability mass function can be written as

$$
\mu^y(1-\mu)^{1-y}=\exp\left\{y\log\frac{\mu}{1-\mu}+\log(1-\mu)\right\}.
$$

Thus $\theta=\log(\mu/(1-\mu))$ and $K(\theta)=\log(1+e^\theta)$. **The canonical link is the logit:**

$$
\boxed{g(\mu)=\log\frac{\mu}{1-\mu},\qquad 0<\mu<1.}
$$

## ↑ Ancestors (10)

1. [5I](../5i.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
