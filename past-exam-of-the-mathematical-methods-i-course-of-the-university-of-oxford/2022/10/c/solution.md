<h1 id="10/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A column of [coordinates](../../../../coordinate-linear-algebra.md) transforms as $\mathbf x'=U^\dagger\mathbf x$, because the columns of $U$ are the new [orthonormal basis](../../../../orthonormal-basis.md) vectors expressed in the old [coordinates](../../../../coordinate-linear-algebra.md). A symmetric unitary choice is

$$
\boxed{U=\frac1{\sqrt2}\begin{pmatrix}1&0&i\\0&\sqrt2&0\\i&0&1\end{pmatrix},\quad
A'=\operatorname{diag}(-1,3,1),\quad
\mathbf x'=\begin{pmatrix}(1-i)/\sqrt2\\1\\(1-i)/\sqrt2\end{pmatrix}.}
$$

Its first and third columns are orthogonal [eigenvectors](../../../../eigenvector.md) of the $xz$ block, with [eigenvalues](../../../../eigenvalue.md) $-1$ and $+1$ respectively; its second column is the $y$ axis with eigenvalue $3$. Direct multiplication checks $U^\dagger U=I$, while the displayed entries give $U^T=U$. The symmetry here means transpose symmetry, not [Hermitian](../../../../hermitian-operator.md) symmetry.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [10](../../10.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
