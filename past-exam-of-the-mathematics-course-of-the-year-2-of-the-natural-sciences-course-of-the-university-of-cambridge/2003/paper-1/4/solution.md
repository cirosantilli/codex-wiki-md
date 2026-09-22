<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [spectral theorem](../../../../spectral-theorem.md) gives a real orthonormal [eigenbasis](../../../../eigenbasis.md) $v_1,\ldots,v_n$ for a real [symmetric matrix](../../../../symmetric-matrix.md) $A$. Distinct [eigenspaces](../../../../eigenspace.md) are [orthogonal](../../../../orthogonal-vectors.md); within a repeated [eigenspace](../../../../eigenspace.md), choose an [orthonormal basis](../../../../orthonormal-basis.md), for example by [Gram-Schmidt orthogonalization](../../../../gram-schmidt-process.md). Put these [eigenvectors](../../../../eigenvector.md) in the columns of $T$. Then $T^{-1}=T^T$ and

$$
T^{-1}AT=\operatorname{diag}(\lambda_1,\ldots,\lambda_n).
$$

For a change of variables $y=Sx$, choose $\boxed{S=T^T}$. Since $x=Ty$, the [quadratic form](../../../../quadratic-form-split.md) becomes $x^TAx=\sum_i\lambda_i y_i^2$; the $\lambda_i$ are precisely the [eigenvalues](../../../../eigenvalue.md) of $A$.

In the numerical case, the off-diagonal entries are half the cross-term coefficients, so

$$
A=\begin{pmatrix}1&1&3\\1&1&-3\\3&-3&-3\end{pmatrix}.
$$

A direct [eigenvector](../../../../eigenvector.md) calculation gives the unit [eigenvectors](../../../../eigenvector.md) $(1,1,0)/\sqrt2$, $(1,-1,1)/\sqrt3$, $(1,-1,-2)/\sqrt6$, with [eigenvalues](../../../../eigenvalue.md) two, three and minus six. They are pairwise [orthogonal](../../../../orthogonal-vectors.md). Therefore the required [orthogonal diagonalization](../../../../orthogonal-diagonalization-of-a-real-symmetric-matrix.md) is

$$
\boxed{y_1=\frac{x_1+x_2}{\sqrt2},\qquad y_2=\frac{x_1-x_2+x_3}{\sqrt3},\qquad y_3=\frac{x_1-x_2-2x_3}{\sqrt6},}
$$

and the transformed [quadratic form](../../../../quadratic-form-split.md) is $\boxed{2y_1^2+3y_2^2-6y_3^2}$.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [Paper 1](../../paper-1-split.md)
3. [2003](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
