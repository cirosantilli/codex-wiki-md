<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Lévy characterization of multidimensional Brownian motion](../../../../../../levy-characterization-of-multidimensional-brownian-motion.md) says that a continuous adapted $\mathbb R^d$-valued process $Z$, with $Z_0=0$, is standard [Brownian motion](../../../../../../brownian-motion-split.md) relative to the given [filtration](../../../../../../filtration-probability-theory.md) if and only if its coordinates are [local martingales](../../../../../../local-martingale.md) and

$$
\boxed{[Z^i,Z^j]_t=\delta_{ij}t\qquad(1\le i,j\le d).}
$$

For [Brownian motion](../../../../../../brownian-motion-split.md), independent centered Gaussian increments give the [martingale](../../../../../../martingale-split.md) property of each coordinate and of $Z_t^iZ_t^j-\delta_{ij}t$. The defining uniqueness of [quadratic covariation](../../../../../../quadratic-covariation.md) consequently gives the bracket condition.

Conversely, suppose the [local martingale](../../../../../../local-martingale.md) and bracket conditions hold. For $\theta\in\mathbb R^d$, the [Itô formula](../../../../../../ito-s-lemma.md) gives

$$
E_t=\exp\left(i\theta\cdot Z_t+\tfrac12|\theta|^2t\right),\qquad dE_t=iE_t\,\theta\cdot dZ_t,
$$

since the bracket term cancels the time derivative. On $[0,T]$, $|E_t|\le e^{|\theta|^2T/2}$, so its real and imaginary parts are bounded [local martingales](../../../../../../local-martingale.md) and hence true [martingales](../../../../../../martingale-split.md). Thus, for $s\le t$,

$$
\mathbb E\left[e^{i\theta\cdot(Z_t-Z_s)}\mid\mathcal F_s\right]=e^{-\frac12|\theta|^2(t-s)}.
$$

This is the [characteristic function](../../../../../../characteristic-function.md) of $N(0,(t-s)I_d)$ and is independent of $\mathcal F_s$. Uniqueness of [characteristic functions](../../../../../../characteristic-function.md) shows that $Z_t-Z_s$ has that [Gaussian distribution](../../../../../../normal-distribution.md) and is independent of the past. Iterating over ordered times gives independent Gaussian increments; together with continuous paths and $Z_0=0$, these are precisely the defining properties of standard [Brownian motion](../../../../../../brownian-motion-split.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
