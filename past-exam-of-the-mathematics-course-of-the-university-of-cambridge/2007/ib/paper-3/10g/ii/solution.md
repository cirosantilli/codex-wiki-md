<h1 id="10g/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Regard $B$ as a [linear map](../../../../../../linear-map.md) $\mathbb R^n\to\mathbb R^p$ and $A$ as a [linear map](../../../../../../linear-map.md) $\mathbb R^p\to\mathbb R^m$ (the same argument holds over any [field](../../../../../../field.md)). Then

$$
\operatorname{im}(AB)=A(\operatorname{im}B)\subseteq\operatorname{im}A.
$$

Its [dimension](../../../../../../dimension-vector-space.md) cannot exceed either $\dim\operatorname{im}A$ or $\dim\operatorname{im}B$, since applying a [linear map](../../../../../../linear-map.md) cannot increase [dimension](../../../../../../dimension-vector-space.md). The [rank bound for a matrix product](../../../../../../rank-bound-for-a-matrix-product.md) is therefore

$$
\boxed{\operatorname{rank}(AB)\leq\min\{\operatorname{rank}A,\operatorname{rank}B\}\leq p.}
$$

The bound $p$ is attained when

$$
A=\begin{pmatrix}I_p\\0_{(m-p)\times p}\end{pmatrix},\qquad B=\begin{pmatrix}I_p&0_{p\times(n-p)}\end{pmatrix}.
$$

Their product has an $I_p$ block and zeros elsewhere, so its [rank of a matrix](../../../../../../matrix-rank.md) is $p$. Thus the bound depending only on the given [matrix](../../../../../../matrix.md) sizes is **sharp**.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [10G](../../10g.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
