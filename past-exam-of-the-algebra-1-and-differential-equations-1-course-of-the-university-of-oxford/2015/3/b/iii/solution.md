<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Proceed by induction on the [dimension](../../../../../dimension-vector-space.md). For positive [dimension](../../../../../dimension-vector-space.md), the [fundamental theorem of algebra](../../../../../fundamental-theorem-of-algebra.md) gives a root of the [characteristic polynomial](../../../../../characteristic-polynomial.md), hence a nonzero [eigenvector](../../../../../eigenvector.md) $v$. Normalize it to have [norm](../../../../../norm.md) one. Its span is an [invariant subspace](../../../../../invariant-subspace.md), and part (ii) makes its [orthogonal complement](../../../../../orthogonal-complement.md) invariant too:

$$
V=\operatorname{span}\{v\}\oplus\operatorname{span}\{v\}^{\perp}.
$$

The restriction of $T$ to the complement remains [skew-adjoint](../../../../../skew-adjoint-generator.md), since the same [inner product](../../../../../inner-product-split.md) identity holds there. The induction hypothesis supplies an [orthonormal eigenbasis](../../../../../orthonormal-eigenbasis.md) for that smaller space. Adjoining $v$ gives an [orthonormal eigenbasis](../../../../../orthonormal-eigenbasis.md) for $V$.

The zero-dimensional base case is immediate. Thus **$T$ is [diagonalizable](../../../../../diagonalizable-matrix.md), indeed unitarily diagonalizable**. This proves the finite-dimensional case of the [spectral theorem](../../../../../spectral-theorem.md) for a [skew-adjoint operator](../../../../../skew-adjoint-generator.md) without assuming that distinct [eigenvalues](../../../../../eigenvalue.md) have multiplicity one.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the algebra 1 and differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Algebra 1 and differential equations 1 course of the University of Oxford](../../../../../algebra-1-and-differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
