<h1 id="22f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [bounded linear operator](../../../../../../continuous-linear-operator.md) $T:X\to Y$ is a [compact operator](../../../../../../compact-operator-split.md) when the image of the closed unit ball has [compact closure](../../../../../../relatively-compact-subset.md), equivalently when every bounded sequence $(x_n)$ has a subsequence for which $(Tx_n)$ converges.

Each $T_i$ is compact because its image lies in a finite-dimensional subspace. Let $B_X$ be the unit ball and fix $\varepsilon>0$. Choose $i$ with $\lVert T-T_i\rVert<\varepsilon/3$. Since $T_i(B_X)$ is relatively compact, it has a finite $\varepsilon/3$-net $y_1,\ldots,y_N$. For each $x\in B_X$, choose $y_j$ with $\lVert T_ix-y_j\rVert<\varepsilon/3$; then

$$
\lVert Tx-y_j\rVert
\leq\lVert(T-T_i)x\rVert+\lVert T_ix-y_j\rVert
<\frac{2\varepsilon}{3}.
$$

Thus $T(B_X)$ is [totally bounded](../../../../../../totally-bounded-space.md). Its closure is complete because $Y$ is a [Banach space](../../../../../../banach-space-split.md), so it is compact. This proves the [norm-closedness of compact operators](../../../../../../norm-closedness-of-compact-operators.md) and hence

$$
\boxed{T\text{ is compact}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
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
