<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Set $A^{(0)}=A$. At step $k=1,\ldots,n-2$, let $u=A^{(k-1)}_{k+1:n,k}$ be the column below the diagonal. Choose a [Householder reflection](../../../../householder-transformation.md) $\widehat H_k$ sending $u$ onto its first coordinate axis, and embed it as

$$
P_k=\operatorname{diag}(I_k,\widehat H_k),\qquad A^{(k)}=P_k^TA^{(k-1)}P_k.
$$

If $u=0$, use $P_k=I$. Left multiplication annihilates entries $k+2,\ldots,n$ in column $k$. Right multiplication performs the matching operation on row $k$, because the [matrix](../../../../matrix.md) remains [symmetric](../../../../symmetric-relation.md). The first $k$ coordinates are fixed, so zeros already created in earlier columns and rows are preserved.

Here the [orthogonality](../../../../orthogonal-vectors.md) of each $P_k$ is used explicitly: $P_k^{-1}=P_k^T$, so each update is a [similarity transformation](../../../../similarity-transformation.md) and preserves [eigenvalues](../../../../eigenvalue.md). After $n-2$ steps,

$$
\boxed{T=Q^TAQ,\qquad Q=P_1P_2\cdots P_{n-2},}
$$

where $Q$ is [orthogonal](../../../../orthogonal-vectors.md) and $T$ is a real symmetric [tridiagonal matrix](../../../../tridiagonal-matrix.md). This is [Householder tridiagonalization](../../../../householder-tridiagonalization.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the numerical analysis course of the University of Oxford](../../../split.md)
5. [Numerical analysis course of the University of Oxford](../../../../numerical-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
