<h1 id="10f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

If $A$ is a [Hermitian matrix](../../../../../../hermitian-operator.md), then $(BAB^*)^*=BAB^*$, so $M_B$ preserves $W$. Addition and multiplication by real [scalars](../../../../../../scalar.md) commute with this operation, making $T_B$ a real [linear map](../../../../../../linear-map.md).

A real [basis](../../../../../../basis.md) of $W$ consists of $E_{ii}$ and, for $i<j$, $E_{ij}+E_{ji}$ and $i(E_{ij}-E_{ji})$. It has $n^2$ elements and is also a complex [basis](../../../../../../basis.md) of all matrices. Indeed every matrix is uniquely $H+iK$ with $H,K$ [Hermitian matrices](../../../../../../hermitian-operator.md), by taking

$$
H=\frac{A+A^*}{2},\qquad K=\frac{A-A^*}{2i}.
$$

Real linear independence of the displayed [basis](../../../../../../basis.md) therefore implies complex linear independence. Since its images under $M_B$ are [Hermitian matrices](../../../../../../hermitian-operator.md), the matrix of $M_B$ in this complex [basis](../../../../../../basis.md) has exactly the same real entries as the matrix of $T_B$ in the real [basis](../../../../../../basis.md). Their [determinants](../../../../../../determinant.md) are equal. **There is no further squaring when passing to this real subspace:**

$$
\boxed{\det T_B=|\det B|^{2n}.}
$$

This is the [determinant of Hermitian congruence](../../../../../../determinant-of-hermitian-congruence.md), including the case of singular $B$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [10F](../../10f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
