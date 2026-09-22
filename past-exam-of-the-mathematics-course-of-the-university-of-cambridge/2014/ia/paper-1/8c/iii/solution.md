<h1 id="8c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For $a=(a_1,a_2,a_3)$ the map has the explicit form

$$
\mathcal M(a)=\frac12\begin{pmatrix}ia_1&a_2+ia_3\\-a_2+ia_3&-ia_1\end{pmatrix}.
$$

Its diagonal entries sum to zero and its [conjugate transpose](../../../../../../conjugate-transpose.md) is its negative, because the three coordinates are real. Hence it is traceless and a [skew-Hermitian matrix](../../../../../../skew-hermitian-matrix.md).

Direct multiplication of the given basis [matrices](../../../../../../matrix.md) yields

$$
[M_1,M_2]=M_3,\qquad[M_2,M_3]=M_1,\qquad[M_3,M_1]=M_2.
$$

The reverse products give the negative [commutators](../../../../../../commutator.md), and equal-index [commutators](../../../../../../commutator.md) vanish. Bilinearity then gives

$$
[\mathcal M(a),\mathcal M(b)]
=(a_2b_3-a_3b_2)M_1+(a_3b_1-a_1b_3)M_2+(a_1b_2-a_2b_1)M_3.
$$

Thus **the [cross product](../../../../../../cross-product.md) is represented by the [commutator](../../../../../../commutator.md)**:

$$
\boxed{\mathcal M(a\times b)=[\mathcal M(a),\mathcal M(b)].}
$$

This realizes the [cross-product model of su(2)](../../../../../../cross-product-model-of-su-2.md) with exactly the normalization and cyclic orientation used here.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [8C](../../8c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
