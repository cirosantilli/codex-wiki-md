<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\pi_0$ be the [probability density function](../../../../../../probability-density-function.md) of the unknown and $\rho$ that of the noise, both relative to [Lebesgue measure](../../../../../../lebesgue-measure.md). By [independence of random variables](../../../../../../independent-random-variables.md), the [conditional distribution](../../../../../../conditional-distribution.md) of the measurement given $u$ has density $\rho(m-Au)$. Thus its [likelihood function](../../../../../../likelihood-function.md) and the joint density are

$$
\pi(m\mid u)=\rho(m-Au),\qquad
\pi(u,m)=\pi_0(u)\rho(m-Au).
$$

The [Bayesian model evidence](../../../../../../bayesian-model-evidence.md) is the marginal data density

$$
Z(m)=\int_{\mathbb R^d}\pi_0(v)\rho(m-Av)\,dv.
$$

[Bayes' theorem](../../../../../../bayes-theorem.md) gives the [posterior density](../../../../../../posterior-density.md) solving this [Bayesian inverse problem](../../../../../../bayesian-inverse-problem.md):

$$
\boxed{\pi^m(u)=\frac{\pi_0(u)\rho(m-Au)}{Z(m)}.}
$$

This formula applies when $0<Z(m)<\infty$. Since $\int Z(m)\,dm=1$ by [Tonelli theorem](../../../../../../tonelli-theorem.md), these conditions hold [almost everywhere](../../../../../../almost-everywhere.md) under the marginal data law. Values of a [conditional distribution](../../../../../../conditional-distribution.md) at exceptional data are not determined by the joint law. The [posterior mean](../../../../../../posterior-mean.md) or a [maximum a posteriori estimate](../../../../../../maximum-a-posteriori-estimate.md) can then give a point estimate, while the full [posterior density](../../../../../../posterior-density.md) describes the remaining uncertainty.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 350](../../../paper-350-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
