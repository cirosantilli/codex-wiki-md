<h1 id="9g/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The $n$ spanning vectors form a [basis](../../../../../../basis.md). Write

$$
T^nx=-a_0x-a_1Tx-\cdots-a_{n-1}T^{n-1}x.
$$

In this cyclic basis the matrix is the [companion matrix](../../../../../../companion-matrix.md)

$$
C=\begin{pmatrix}0&0&\cdots&0&-a_0\\1&0&\cdots&0&-a_1\\0&1&\cdots&0&-a_2\\\vdots&\vdots&\ddots&\vdots&\vdots\\0&0&\cdots&1&-a_{n-1}\end{pmatrix}.
$$

Expanding $\det(tI-C)$ along its last column gives

$$
\chi_T(t)=t^n+a_{n-1}t^{n-1}+\cdots+a_1t+a_0.
$$

For example, the term containing $a_j$ has minor $t^j$ and the signs from the subdiagonal cancel the cofactor sign; the diagonal term supplies $t^n$. The defining relation says $\chi_T(T)x=0$. Every polynomial in $T$ commutes with $T$, so

$$
\chi_T(T)T^jx=T^j\chi_T(T)x=0\qquad(0\leq j<n).
$$

It therefore vanishes on a [basis](../../../../../../basis.md), proving

$$
\boxed{\chi_T(T)=0.}
$$

This direct argument for a [cyclic vector](../../../../../../cyclic-vector.md) does not assume the [Cayley-Hamilton theorem](../../../../../../cayley-hamilton-theorem.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [9G](../../9g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
