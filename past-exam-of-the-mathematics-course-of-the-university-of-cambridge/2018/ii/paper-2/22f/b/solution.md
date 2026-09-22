<h1 id="22f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $K=\overline{T(B_X)}$, which is compact. Every $y^*$ in the unit ball of the [continuous dual space](../../../../../../continuous-dual-space-split.md) $Y^*$ restricts to a function on $K$. These functions are uniformly bounded and equicontinuous, since

$$
|y^*(z)-y^*(w)|\leq\lVert z-w\rVert.
$$

By the [Arzelà-Ascoli theorem](../../../../../../arzela-ascoli-theorem.md), every sequence $(y_n^*)$ in the unit ball has a subsequence that converges uniformly on $K$. Along this subsequence,

$$
\lVert T^*y_n^*-T^*y_m^*\rVert
=\sup_{x\in B_X}|(y_n^*-y_m^*)(Tx)|
\leq\sup_{z\in K}|(y_n^*-y_m^*)(z)|\longrightarrow0.
$$

The [continuous dual space](../../../../../../continuous-dual-space-split.md) $X^*$ is complete, so $(T^*y_n^*)$ converges in norm. Every sequence in the image of the unit ball therefore has a convergent subsequence, proving the forward direction of the [Schauder theorem for compact operators](../../../../../../schauder-theorem-for-compact-operators.md):

$$
\boxed{T^*:Y^*\to X^*\text{ is compact}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [22F](../../22f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
