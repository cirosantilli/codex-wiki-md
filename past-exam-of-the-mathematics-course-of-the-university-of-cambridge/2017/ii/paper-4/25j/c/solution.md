<h1 id="25j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Birkhoff ergodic theorem](../../../../../../birkhoff-ergodic-theorem.md) states: for a [measure-preserving transformation](../../../../../../measure-preserving-transformation.md) $\theta$ of a [finite measure](../../../../../../finite-measure.md) space and $f\in L^1$, the averages $A_nf=n^{-1}\sum_{j=0}^{n-1}f\circ\theta^j$ converge [almost everywhere](../../../../../../almost-everywhere.md) and in $L^1$ to an invariant function $f^*$. On a [probability space](../../../../../../probability-space.md),

$$
\boxed{f^*=\mathbb E[f\mid\mathcal I],}
$$

where $\mathcal I$ is the [invariant sigma-algebra](../../../../../../invariant-sigma-algebra.md) modulo null sets. In particular the integral is preserved, and if $\theta$ is ergodic then $f^*=\int f\,d\mu$ [almost everywhere](../../../../../../almost-everywhere.md); for a finite space of nonunit mass, this constant is $\mu(E)^{-1}\int f\,d\mu$ when $\mu(E)>0$.

The [maximal ergodic lemma](../../../../../../maximal-ergodic-lemma.md) says that for real integrable $f$, with $S_kf=\sum_{j=0}^{k-1}f\circ\theta^j$ and $E_N=\{\max_{1\leq k\leq N}S_kf>0\}$,

$$
\boxed{\int_{E_N}f\,d\mu\geq0.}
$$

The same inequality holds on $E_\infty=\{\sup_{k\geq1}S_kf>0\}$, by taking the increasing [limit](../../../../../../limit-of-a-function.md) and dominated convergence. These statements do not require the transformation to be invertible or the space to be ergodic.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [25J](../../25j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
