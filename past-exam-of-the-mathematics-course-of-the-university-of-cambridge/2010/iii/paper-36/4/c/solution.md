<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The bounded uniform [prior distributions](../../../../../../prior-probability.md) on the slopes and population intercept are proper and broad on their stated scale. They allow either sign but are not invariant to changes of units. The residual [precision parameter](../../../../../../precision-parameter.md) $q=1/\sigma^2$ has a proper shape-rate $\operatorname{Gamma}(0.001,0.001)$ prior. Equivalently, $\sigma^2$ has [inverse-gamma distribution](../../../../../../inverse-gamma-distribution.md) with the same shape and scale. This is a commonly used diffuse choice, but it is not literally noninformative and its tail behaviour merits sensitivity analysis.

The prior for $\tau$ is uniform on $(0,100)$, so the induced density of $v=\tau^2$ is

$$
\boxed{\pi(v)=\frac1{200\sqrt v},\qquad0<v<10000.}
$$

It is integrable at zero, unlike the usual scale-invariant variance kernel $\pi(v)\propto1/v$. The latter kernel, often called the standard variance [Jeffreys prior](../../../../../../jeffreys-prior.md), would cause an [improper posterior from a log-uniform random-effect scale prior](../../../../../../improper-posterior-from-a-log-uniform-random-effect-scale-prior.md) here. After integrating the child intercepts, each child's response vector has a normal likelihood with [covariance matrix](../../../../../../covariance-matrix.md) $\sigma^2I_3+v\mathbf1\mathbf1^T$. For fixed positive $\sigma^2$, this covariance remains nonsingular at $v=0$, and the marginal likelihood has a positive finite limit there. On a compact set of the other parameters its positivity gives

$$
\int_0^\varepsilon L(v)\frac{dv}{v}=\infty.
$$

Consequently the scale-invariant kernel cannot be normalized to a [posterior distribution](../../../../../../bayesian-posterior.md). A proper prior on the standard deviation avoids this problem. This familiar scale prior is not necessarily the actual [Jeffreys prior for an additive variance component](../../../../../../jeffreys-prior-for-an-additive-variance-component.md) derived from the observed-data likelihood; the latter can be finite at zero.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
