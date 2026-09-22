<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The matrix is real symmetric, so the [spectral theorem](../../../spectral-theorem.md) guarantees an [orthonormal basis](../../../orthonormal-basis.md) of [eigenvectors](../../../eigenvector.md). Its characteristic determinant factors as

$$
\det(A-\lambda I)=-(\lambda+3)(\lambda-6)(\lambda-1).
$$

Solving the three corresponding equations for the [null space](../../../kernel-of-a-linear-map-split.md) gives the normalized [eigenvectors](../../../eigenvector.md)

$$
\boxed{\lambda=6:\ \frac1{\sqrt5}\begin{pmatrix}2\\0\\-1\end{pmatrix},\qquad\lambda=-3:\ \begin{pmatrix}0\\1\\0\end{pmatrix},\qquad\lambda=1:\ \frac1{\sqrt5}\begin{pmatrix}1\\0\\2\end{pmatrix}.}
$$

Their pairwise [inner products](../../../inner-product-split.md) vanish. With these vectors as columns,

$$
Q=\begin{pmatrix}2/\sqrt5&0&1/\sqrt5\\0&1&0\\-1/\sqrt5&0&2/\sqrt5\end{pmatrix},\qquad\boxed{Q^TAQ=\operatorname{diag}(6,-3,1).}
$$

Since $Q^TQ=I$, this also gives $A=Q\operatorname{diag}(6,-3,1)Q^T$.

## ↑ Ancestors (11)

1. [4](../4.md)
2. [2015 resit](../../2015-resit-split.md)
3. [Past exam of the mathematical methods I course of the University of Oxford](../../split.md)
4. [Mathematical methods I course of the University of Oxford](../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
