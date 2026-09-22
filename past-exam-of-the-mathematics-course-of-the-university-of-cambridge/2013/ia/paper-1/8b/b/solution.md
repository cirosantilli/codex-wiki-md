<h1 id="8b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let the repeated [eigenvalue](../../../../../../eigenvalue.md) be $a$, and choose an [eigenvector](../../../../../../eigenvector.md) $v_1\ne0$. Complete it to a basis $(v_1,v_2)$ of $\mathbb C^2$. In this basis the matrix is an [upper triangular matrix](../../../../../../upper-triangular-matrix.md), with first column $(a,0)^T$, say $T=\begin{pmatrix}a&c\\0&d\end{pmatrix}$. Its [characteristic polynomial](../../../../../../characteristic-polynomial.md) is $(t-a)(t-d)$. By part (a)(ii), this must equal $(t-a)^2$, so $d=a$.

If $c=0$, the matrix is already $aI$. If $c\ne0$, rescale the first basis vector by $k=c$ and apply part (a)(iii); the upper-right entry becomes one. Thus

$$
\boxed{M\sim aI\quad\text{or}\quad M\sim\begin{pmatrix}a&1\\0&a\end{pmatrix}.}
$$

The second possibility is a size-two [Jordan block](../../../../../../jordan-block.md). It has only one independent [eigenvector](../../../../../../eigenvector.md), whereas $aI$ has a two-dimensional eigenspace, so the two types cannot be related by [matrix similarity](../../../../../../matrix-similarity.md). This [repeated-eigenvalue classification in dimension two](../../../../../../repeated-eigenvalue-classification-in-dimension-two.md) proves the required result without assuming the general [Jordan normal form](../../../../../../jordan-normal-form.md) theorem.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [8B](../../8b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
