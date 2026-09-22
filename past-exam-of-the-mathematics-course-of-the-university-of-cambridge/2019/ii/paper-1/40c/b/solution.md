<h1 id="40c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Here $D=I$, so the Jacobi iteration matrix is

$$
H=I-A=
\begin{pmatrix}
0&-\alpha&-\alpha\\
-\alpha&0&-\alpha\\
-\alpha&-\alpha&0
\end{pmatrix}.
$$

The all-ones vector is an [eigenvector](../../../../../../eigenvector.md) with [eigenvalue](../../../../../../eigenvalue.md) $-2\alpha$. On its two-dimensional [orthogonal complement](../../../../../../orthogonal-complement.md), the coordinates sum to zero and $Hv=\alpha v$, so the other eigenvalue is $\alpha$ with multiplicity two. Therefore

$$
\rho(H)=\max\{2|\alpha|,|\alpha|\}=2|\alpha|.
$$

By [Jacobi convergence for a three-by-three equicorrelation matrix](../../../../../../jacobi-convergence-for-a-three-by-three-equicorrelation-matrix.md), convergence occurs exactly for

$$
\boxed{-\frac12<\alpha<\frac12.}
$$

At either endpoint the spectral radius is one, so convergence for arbitrary initial data fails.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [40C](../../40c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
