<h1 id="16e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $d_n(x)=\det(xI-A_n)$, and set $d_0=1$, $d_1=x-a_1$. Expansion of the tridiagonal [determinant](../../../../../../determinant.md) along its last row gives

$$
d_n=(x-a_n)d_{n-1}-b_n^2d_{n-2}.
$$

For the second term, the last-row entry is $-b_n$, its cofactor has negative sign, and the remaining minor has last-column entry $-b_n$ multiplying $d_{n-2}$; their product is $-b_n^2d_{n-2}$. Thus $d_n$ and $p_n$ have identical initial values and recurrence, and induction proves

$$
\boxed{p_n(x)=\det(xI-A_n).}
$$

The [eigenvalues](../../../../../../eigenvalue.md) of the [Jacobi matrix](../../../../../../jacobi-matrix.md) $A_n$ are precisely the roots of this [characteristic polynomial](../../../../../../characteristic-polynomial.md). Part(a) therefore gives **all $n$ eigenvalues simple and lying strictly in $(a,b)$**. This conclusion follows from orthogonality as well as symmetry; symmetry alone would establish real eigenvalues but not their interval location.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [16E](../../16e.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
