<h1 id="2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use the product from part (ii). Move each selected element of each small set $X_i$ to the left, conjugating every approximate-group factor that it crosses. For each tuple $\mathbf x\in X_1\times\cdots\times X_m$, the corresponding part of the product is therefore contained in

$$
y_{\mathbf x}D_{1,\mathbf x}\cdots D_{n,\mathbf x},
$$

where every $D_{j,\mathbf x}$ is a [conjugate subset](../../../../../../../conjugate-subset.md) of some $C_j$. Conjugation preserves cardinality, the approximation parameter, and the property that the generated subgroup is abelian. The conjugating elements belong to $A^{O_s(1)}$, so $D_{j,\mathbf x}\subseteq A^{O_s(1)}$ after enlarging the implicit constant.

The number of tuples is at most

$$
\prod_{i=1}^m|X_i|
\leq\exp\bigl(O_s(\log^{O_s(1)}(2K))\bigr).
$$

These translated products cover $A$, so one has size at least the reciprocal fraction of $|A|$. For that tuple, put $D_j=D_{j,\mathbf x}$. Then

$$
\boxed{|D_1\cdots D_q|
\geq\exp\bigl(-O_s(\log^{O_s(1)}(2K))\bigr)|A|,}
$$

where $q=n\leq O_s(\log^{O_s(1)}(2K))$, and each $D_j$ is a $K^{O_s(1)}$-approximate group generating an [abelian subgroup](../../../../../../../abelian-subgroup.md).

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 149](../../../../paper-149-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
