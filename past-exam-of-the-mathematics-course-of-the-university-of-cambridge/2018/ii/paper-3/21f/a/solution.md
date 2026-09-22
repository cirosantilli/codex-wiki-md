<h1 id="21f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $(T_m)$ be Cauchy in the [operator norm](../../../../../../operator-norm.md) on $\mathcal B(X,Y)$. For each $x\in X$,

$$
\lVert T_mx-T_lx\rVert
\leq\lVert T_m-T_l\rVert\,\lVert x\rVert,
$$

so $(T_mx)$ is Cauchy in the [Banach space](../../../../../../banach-space-split.md) $Y$. Define

$$
Tx=\lim_{m\to\infty}T_mx.
$$

Pointwise passage to the limit shows that $T$ is linear. A norm-Cauchy sequence is bounded, say $\lVert T_m\rVert\leq M$, and hence

$$
\lVert Tx\rVert\leq M\lVert x\rVert.
$$

Thus $T$ is bounded. Finally, for fixed $m$,

$$
\lVert(T_m-T)x\rVert
=\lim_{l\to\infty}\lVert(T_m-T_l)x\rVert
\leq\left(\limsup_{l\to\infty}\lVert T_m-T_l\rVert\right)\lVert x\rVert.
$$

The right-hand coefficient tends to zero with $m$, so $T_m\to T$ in operator norm. Therefore

$$
\boxed{\mathcal B(X,Y)\text{ is a Banach space}.}
$$

This is the [Banach space of bounded linear operators](../../../../../../banach-space-of-bounded-linear-operators.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [21F](../../21f.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
