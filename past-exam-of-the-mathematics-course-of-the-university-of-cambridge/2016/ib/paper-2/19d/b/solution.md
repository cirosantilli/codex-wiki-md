<h1 id="19d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [QR decomposition](../../../../../../qr-decomposition.md) of an $m\times n$ matrix, $m\ge n$, is $A=QR$, where $Q$ is an $m\times m$ [orthogonal matrix](../../../../../../orthogonal-matrix.md) and $R$ is $m\times n$ and upper trapezoidal: $R_{ij}=0$ for $i>j$. In particular its bottom $m-n$ rows vanish.

Successive left [Givens rotations](../../../../../../givens-rotation.md) annihilate the entries below the diagonal, column by column. When working on column $j$, rotate rows $j$ and $i>j$; their earlier columns are already zero, so the earlier eliminations persist. If $G_k\cdots G_1A=R$, then

$$
\boxed{Q=G_1^T\cdots G_k^T,\qquad A=QR.}
$$

A product of [orthogonal matrices](../../../../../../orthogonal-matrix.md) is orthogonal. The construction remains valid for a rank-deficient matrix, although uniqueness is not asserted. This is [QR decomposition by Givens rotations](../../../../../../qr-decomposition-by-givens-rotations.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [19D](../../19d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
