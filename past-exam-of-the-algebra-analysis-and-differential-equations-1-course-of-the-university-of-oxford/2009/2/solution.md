<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [self-adjoint operator](../../../self-adjoint-operator.md) satisfies $\langle Tx,y\rangle=\langle x,Ty\rangle$ for every $x,y$. The finite-dimensional [finite-dimensional spectral theorem](../../../finite-dimensional-spectral-theorem.md) gives an [orthonormal basis](../../../orthonormal-basis.md) of [eigenvectors](../../../eigenvector.md) and real [eigenvalues](../../../eigenvalue.md); [eigenvectors](../../../eigenvector.md) for distinct [eigenvalues](../../../eigenvalue.md) are orthogonal. Consequently a matrix represents a self-adjoint transformation in some, possibly nonorthonormal, basis exactly when it is [diagonalizable](../../../diagonalizable-matrix.md) with real [eigenvalues](../../../eigenvalue.md).

For $A_0$, the [eigenvalues](../../../eigenvalue.md) are $2,1,0$, all distinct and real. Eigenvectors are $e_1$, $e_2$, and $(0,-1,1)^T$. Thus **$A_0$ can represent a self-adjoint transformation** after choosing a suitable basis.

For $A_1$, the eigenvalue one has algebraic multiplicity two but its [eigenspace](../../../eigenspace.md) has dimension one. The lower $2\times2$ block is a nontrivial [Jordan block](../../../jordan-block.md), so the matrix is not [diagonalizable](../../../diagonalizable-matrix.md). Hence **$A_1$ cannot represent a self-adjoint transformation** in any basis.

For $A_2$, the [eigenspace](../../../eigenspace.md) for two is spanned by $e_1$ and $(0,1,1)^T$, and the eigenvalue-one [eigenspace](../../../eigenspace.md) is spanned by $e_2$. These three vectors form an [eigenbasis](../../../eigenbasis.md). Therefore **$A_2$ can represent a self-adjoint transformation**. To see sufficiency on the given [inner product space](../../../inner-product-space.md), first define the real diagonal transformation in an [orthonormal basis](../../../orthonormal-basis.md) and then apply the inverse of a diagonalizing basis change to obtain the requested matrix. Symmetry of the displayed matrix itself would be required only for an orthonormal representing basis.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [2009](../../2009-split.md)
3. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../split.md)
4. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
