<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Write $D_k=M_k-M_{k-1}$ for the [martingale difference sequence](../../../../../../martingale-difference-sequence.md). [Bounded increments](../../../../../../bounded-increments.md) mean that one deterministic $C<\infty$ satisfies $|D_k|\leq C$ for every $k$, almost surely. Then $\mathbb E D_k=0$ and, for $j<k$,

$$
\mathbb E[D_jD_k]
=\mathbb E\left[D_j\mathbb E[D_k\mid\mathcal F_{k-1}]\right]=0.
$$

The increments are [uncorrelated random variables](../../../../../../uncorrelated-random-variables.md), uniformly bounded in $L^2$. Applying the supplied [strong law for uniformly L2-bounded uncorrelated random variables](../../../../../../strong-law-for-uniformly-l2-bounded-uncorrelated-random-variables.md) gives $n^{-1}\sum_{k=1}^nD_k\to0$ almost surely. Also $M_0/n\to0$, because $M_0$ is finite almost surely. Therefore **a martingale with [bounded increments](../../../../../../bounded-increments.md) has zero linear growth**:

$$
\boxed{\frac{M_n}{n}\longrightarrow0\quad\text{almost surely}.}
$$

This is the [strong law for martingales with bounded increments](../../../../../../strong-law-for-martingales-with-bounded-increments.md).

For the [submartingale](../../../../../../submartingale.md), let $\Delta Y_k=Y_k-Y_{k-1}$ and define its predictable drift and compensator by

$$
a_k=\mathbb E[\Delta Y_k\mid\mathcal F_{k-1}]\geq0,
\qquad A_n=\sum_{k=1}^na_k,
\qquad N_n=Y_n-A_n.
$$

This is the [Doob decomposition in discrete time](../../../../../../doob-decomposition-theorem.md). The process $N_n$ is a [martingale](../../../../../../martingale-split.md). Since $|\Delta Y_k|\leq C$, we have $0\leq a_k\leq C$, so $|N_k-N_{k-1}|\leq2C$. The result just proved gives $N_n/n\to0$ almost surely, and $A_n\geq0$. Consequently the [strong law for submartingales with bounded increments](../../../../../../strong-law-for-submartingales-with-bounded-increments.md) is

$$
\boxed{\liminf_{n\to\infty}\frac{Y_n}{n}\geq0\quad\text{almost surely}.}
$$

The compensator may grow, so the conclusion is a lower bound rather than a claim of convergence to zero.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
