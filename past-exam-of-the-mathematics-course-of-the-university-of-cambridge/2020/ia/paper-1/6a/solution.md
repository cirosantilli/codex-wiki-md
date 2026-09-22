<h1 id="6a/solution">Solution</h1>

↑ **Parent:** [6A](../6a.md)

A matrix is [Hermitian](../../../../../hermitian-operator.md) when $A^\dagger=A$, and [unitary](../../../../../unitary-matrix.md) when $U^\dagger U=UU^\dagger=I$.

If $A\mathbf u=\lambda\mathbf u$ with $\mathbf u\ne0$, then

$$
\lambda\,\mathbf u^\dagger\mathbf u
=\mathbf u^\dagger A\mathbf u
=(\mathbf u^\dagger A\mathbf u)^*
=\lambda^*\mathbf u^\dagger\mathbf u,
$$

so every [eigenvalue](../../../../../eigenvalue.md) is real. If $A\mathbf u=\lambda\mathbf u$ and $A\mathbf v=\mu\mathbf v$, then

$$
\mu\mathbf u^\dagger\mathbf v
=\mathbf u^\dagger A\mathbf v
=(A\mathbf u)^\dagger\mathbf v
=\lambda\mathbf u^\dagger\mathbf v.
$$

Distinct eigenvalues therefore have [orthogonal eigenvectors](../../../../../orthogonal-vectors.md).

The normalized eigenvectors form an [orthonormal basis](../../../../../orthonormal-basis.md), so the matrix $U=(\mathbf u_1\ \cdots\ \mathbf u_n)$ satisfies $U^\dagger U=I$ and is unitary. With

$$
D=\operatorname{diag}(\lambda_1,\ldots,\lambda_n),
$$

the equations $A\mathbf u_j=\lambda_j\mathbf u_j$ say $AU=UD$, hence $A=UDU^\dagger$. This is the finite-dimensional [unitary diagonalization of a normal matrix](../../../../../unitary-diagonalization-of-a-normal-matrix.md).

A unitary conjugate of an arbitrary [diagonal matrix](../../../../../diagonal-matrix.md) need not be Hermitian: $U=(1)$ and $D=(i)$ give $UDU^\dagger=(i)$. It is Hermitian exactly when all diagonal entries of $D$ are real.

For the displayed matrix, one valid decomposition is

$$
\boxed{
U=\begin{pmatrix}
 i/\sqrt2&0&-i/\sqrt2\\
 0&1&0\\
 1/\sqrt2&0&1/\sqrt2
\end{pmatrix},
\qquad
D=\operatorname{diag}(5,2,-1)}.
$$

The columns are orthonormal eigenvectors, so direct multiplication gives $UDU^\dagger=A$.

## ↑ Ancestors (10)

1. [6A](../6a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
