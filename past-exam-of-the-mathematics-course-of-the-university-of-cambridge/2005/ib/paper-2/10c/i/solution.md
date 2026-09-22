<h1 id="10c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a complex square [matrix](../../../../../../matrix.md), define its [determinant](../../../../../../determinant.md) by

$$
\det A=\sum_{\sigma\in S_n}\operatorname{sgn}(\sigma)\prod_{i=1}^na_{i,\sigma(i)}.
$$

The [cofactor](../../../../../../cofactor.md) is $C_{ij}=(-1)^{i+j}\det A^{(ij)}$, where $A^{(ij)}$ deletes row $i$ and column $j$. The adjugate is the transposed [cofactor matrix](../../../../../../cofactor-matrix.md), $\operatorname{adj}(A)_{ij}=C_{ji}$.

The $(i,j)$ entry of $\operatorname{adj}(A)A$ is $\sum_kC_{ki}a_{kj}$. For $j=i$, expansion along column $i$ gives $\det A$. For $j\ne i$, this same sum is the [determinant](../../../../../../determinant.md) of the [matrix](../../../../../../matrix.md) obtained by replacing column $i$ by column $j$: deleting the replaced column leaves all its [cofactors](../../../../../../cofactor.md) unchanged. The new [matrix](../../../../../../matrix.md) has two equal columns, so its [determinant](../../../../../../determinant.md) is zero. Thus

$$
\boxed{\operatorname{adj}(A)A=(\det A)I_n.}
$$

This proof does not assume invertibility and therefore also covers singular [matrices](../../../../../../matrix.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [10C](../../10c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
