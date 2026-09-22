<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Brownian reflection principle](../../../../../../reflection-principle-wiener-process.md), applied to the negative increments of the [Brownian motion](../../../../../../brownian-motion-split.md) started at $a$, gives

$$
\mathbb P(T_0>t)=2\Phi(a/\sqrt t)-1\longrightarrow0,
$$

where $\Phi$ is the [standard normal distribution function](../../../../../../standard-normal-distribution-function.md). Hence $T_0<\infty$ [almost surely](../../../../../../almost-sure-convergence.md). The stopped [Brownian motion](../../../../../../brownian-motion-split.md) $M_t=B_{t\wedge T_0}$ is a continuous nonnegative [martingale](../../../../../../martingale-split.md), starts at $a$, and eventually vanishes. The [maximal identity for a continuous nonnegative local martingale tending to zero](../../../../../../maximal-identity-for-a-continuous-nonnegative-local-martingale-tending-to-zero.md) therefore gives, for $H=\sup_{0\leq t\leq T_0}B_t$,

$$
\mathbb P(H\geq x)=\begin{cases}1,&0<x\leq a,\\a/x,&x>a.\end{cases}
$$

Equivalently,

$$
\boxed{H\stackrel d=\frac aU,\qquad F_H(x)=\begin{cases}0,&x<a,\\1-a/x,&x\geq a,\end{cases}\qquad f_H(x)=\frac a{x^2}\mathbf1_{\{x>a\}}.}
$$

There is no atom at $a$. This is the [Pareto distribution](../../../../../../pareto-distribution.md) of shape one, or the translated version of the [maximum before a lower Brownian barrier](../../../../../../maximum-before-a-lower-brownian-barrier.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
