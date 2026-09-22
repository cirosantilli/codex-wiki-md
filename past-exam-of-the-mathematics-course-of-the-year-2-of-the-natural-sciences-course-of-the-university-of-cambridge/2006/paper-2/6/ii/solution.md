<h1 id="6/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The unique symmetric and antisymmetric decomposition is $S=(T+T^T)/2$, $A=(T-T^T)/2$. Both pieces are [Cartesian tensors](../../../../../cartesian-tensor.md): transposing $T'=RTR^T$ gives $(T')^T=RT^TR^T$, so $S'=RSR^T$ and $A'=RAR^T$. Hence this is a decomposition into a [symmetric tensor](../../../../../symmetric-tensor.md) and an [antisymmetric second-rank tensor](../../../../../antisymmetric-second-rank-tensor.md), rather than just a decomposition of numerical arrays.

For the [axial vector of an antisymmetric second-rank tensor](../../../../../axial-vector-of-an-antisymmetric-second-rank-tensor.md), contract the two [Levi-Civita symbols](../../../../../levi-civita-symbol.md):

$$
\epsilon_{kij}a_k=\frac12\epsilon_{kij}\epsilon_{klm}A_{lm}=\frac12(\delta_{il}\delta_{jm}-\delta_{im}\delta_{jl})A_{lm}=A_{ij}.
$$

Thus

$$
\boxed{A=\begin{pmatrix}0&a_3&-a_2\\-a_3&0&a_1\\a_2&-a_1&0\end{pmatrix}.}
$$

With this convention $Ax=x\times a$, so the displayed matrix is the negative of the [cross-product matrix](../../../../../cross-product-matrix.md) for $a\times x$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [6](../../6.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
