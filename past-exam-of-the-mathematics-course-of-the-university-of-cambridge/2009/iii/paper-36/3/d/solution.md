<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The regression coefficients have independent proper [uniform distributions](../../../../../../continuous-uniform-distribution.md) on very wide finite intervals. These are flat in the coefficients, not flat in fitted rates, and can be highly informative on the rate scale. The scale $\tau$ is uniform on $(0,100)$, and [WinBUGS](../../../../../../winbugs.md) receives the corresponding precision $1/\tau^2$ for each [normal distribution](../../../../../../normal-distribution.md) random effect. Writing $v=\tau^2$, the induced [prior density](../../../../../../prior-density.md) is

$$
\boxed{p(v)=\frac1{200\sqrt v}\mathbf1_{(0,10000)}(v).}
$$

It is proper and integrable at zero.

The usual scale-invariant variance prior $p(v)\propto1/v$ would instead cause an [improper posterior from a log-uniform random-effect scale prior](../../../../../../improper-posterior-from-a-log-uniform-random-effect-scale-prior.md). After integrating out the plate effects, the [likelihood function](../../../../../../likelihood-function.md) tends as $v\downarrow0$ to the ordinary positive Poisson likelihood. On any compact interior set of coefficient values this limit is positive and bounded away from zero. Hence the posterior normalizing integral contains a divergent factor $\int_0^\varepsilon dv/v$. There is no [posterior distribution](../../../../../../bayesian-posterior.md) under that prior, even if formal full conditional distributions appear usable. Thus **a proper prior with integrable mass near zero is needed here**. The reciprocal-scale rule is the standard pure-scale [Jeffreys prior](../../../../../../jeffreys-prior.md); it should not be confused with the model-specific information prior for an additive variance component.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
