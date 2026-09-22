<h1 id="1/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For an efficient [QR algorithm](../../../../../qr-algorithm.md), first reduce a general real [matrix](../../../../../matrix.md) to [upper Hessenberg matrix](../../../../../upper-hessenberg-matrix.md) by [orthogonal](../../../../../orthogonal-vectors.md) similarities. For a real [symmetric matrix](../../../../../symmetric-matrix.md), use [Householder tridiagonalization](../../../../../householder-tridiagonalization.md); the resulting symmetric [tridiagonal matrix](../../../../../tridiagonal-matrix.md) is the usual input in this setting. These structures are preserved by suitable [QR algorithm](../../../../../qr-algorithm.md) implementations and greatly reduce the work per iteration.

The output is the [eigenvalues](../../../../../eigenvalue.md), together with an [orthogonal](../../../../../orthogonal-vectors.md) reduction when the factors are accumulated. In the symmetric case the target is a diagonal [matrix](../../../../../matrix.md), whose diagonal entries are the real [eigenvalues](../../../../../eigenvalue.md); the accumulated orthogonal columns are [eigenvectors](../../../../../eigenvector.md). For a general real [matrix](../../../../../matrix.md), the target is the real form in a [Schur decomposition](../../../../../schur-decomposition.md): an upper block triangular [matrix](../../../../../matrix.md) with diagonal blocks of size one or two. The two-by-two blocks represent complex conjugate [eigenvalue](../../../../../eigenvalue.md) pairs. An arbitrary unshifted iteration need not converge, so these describe the intended converged output, with appropriate shifts and [block deflation in the QR algorithm](../../../../../block-deflation-in-the-qr-algorithm.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [1](../../../1.md)
4. [2014](../../../../2014-split.md)
5. [Past exam of the numerical analysis course of the University of Oxford](../../../../split.md)
6. [Numerical analysis course of the University of Oxford](../../../../../numerical-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
