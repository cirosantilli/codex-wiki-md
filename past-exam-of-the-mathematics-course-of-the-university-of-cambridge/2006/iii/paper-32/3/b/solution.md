<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

On a product extension of the [probability space](../../../../../../probability-space.md), take a [uniform distribution](../../../../../../continuous-uniform-distribution.md) variable $U$ on $(0,1)$ independent of the original [sigma-algebra](../../../../../../sigma-algebra.md). For $x>0$,

$$
\mathbb P(M_0/U\geq x\mid\mathcal F_0)
=\mathbb P(U\leq M_0/x\mid\mathcal F_0)
=1\wedge\frac{M_0}{x}.
$$

These are the same conditional tails as in the [maximal identity for a continuous nonnegative local martingale tending to zero](../../../../../../maximal-identity-for-a-continuous-nonnegative-local-martingale-tending-to-zero.md). Taking [expectations](../../../../../../expected-value.md) identifies the unconditional [probability distributions](../../../../../../probability-distribution.md):

$$
\boxed{M^*\ \stackrel{d}{=}\ M_0/U.}
$$

If $M_0=0$, define $M_0/U=0$; the endpoint $U=0$ is a null event if one uses $[0,1]$ instead. The possible atom at zero has mass $\mathbb P(M_0=0)$, since the conditional probability of a positive maximum is zero exactly on that event. For fixed $M_0=m>0$, the conditional law is the [Pareto distribution](../../../../../../pareto-distribution.md) of shape one and minimum $m$, with density $m/x^2$ on $x>m$.

## ↑ Ancestors (11)

1. [B](../b.md)
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
