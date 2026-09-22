<h1 id="7b/solution">Solution</h1>

↑ **Parent:** [7B](../7b.md)

A [matrix](../../../../../matrix.md) is a [diagonalizable matrix](../../../../../diagonalizable-matrix.md) if there is an invertible matrix $P$ for which $P^{-1}MP$ is diagonal. Its columns then form a [basis](../../../../../basis.md) of [eigenvectors](../../../../../eigenvector.md), and the diagonal entries are their corresponding [eigenvalues](../../../../../eigenvalue.md).

Here the given eigenvectors form an [orthonormal basis](../../../../../orthonormal-basis.md). Put them into the columns of $Q$:

$$
Q=(\mathbf e_1\ \cdots\ \mathbf e_n),\qquad Q^TQ=I,\qquad Q^{-1}=Q^T.
$$

Define $\Lambda=Q^TMQ$. Its entries are

$$
\Lambda_{ab}=\mathbf e_a^TM\mathbf e_b
=\lambda_b\,\mathbf e_a\cdot\mathbf e_b
=\lambda_b\delta_{ab}.
$$

This proves the claimed [diagonalization of a matrix](../../../../../diagonalization-of-a-matrix.md), rather than merely guessing it:

$$
\boxed{\Lambda=\operatorname{diag}(\lambda_1,\ldots,\lambda_n),\qquad
M=Q\Lambda Q^T.}
$$

The [trace](../../../../../matrix-trace.md) follows directly from this factorization:

$$
\operatorname{tr}M
=\sum_i\sum_a\lambda_aQ_{ia}^2
=\sum_a\lambda_a\sum_iQ_{ia}^2
=\sum_a\lambda_a,
$$

because each column of $Q$ has unit length. **Trace is the sum of the eigenvalues, with multiplicity.**

For the particular matrix, $(M^2)_{ij}=\sum_kM_{ik}M_{kj}$. If $i=j$, every $k\ne i$ contributes one and $k=i$ contributes zero. If $i\ne j$, precisely $k=i$ and $k=j$ contribute zero; the other $n-2$ terms contribute one. Thus

$$
(M^2)_{ij}=
\begin{cases}
n-1,&i=j,\\
n-2,&i\ne j,
\end{cases}
\qquad
M^2=(n-1)I+(n-2)M.
$$

Applying this identity to a nonzero [eigenvector](../../../../../eigenvector.md) gives

$$
\lambda^2=(n-1)+(n-2)\lambda,
\qquad
(\lambda-(n-1))(\lambda+1)=0.
$$

Every [eigenvalue](../../../../../eigenvalue.md) is therefore $n-1$ or $-1$.

If $r$ is the multiplicity of $n-1$, the [trace](../../../../../matrix-trace.md) formula for a [diagonalizable matrix](../../../../../diagonalizable-matrix.md) and the zero diagonal give

$$
0=r(n-1)+(n-r)(-1)=n(r-1),
$$

so $r=1$. Up to ordering, the required diagonal form is

$$
\boxed{\Lambda=\operatorname{diag}(n-1,-1,\ldots,-1).}
$$

For $n=1$ this means just $(0)$. For $n\ge2$, the eigendirections are also transparent: the all-ones vector has eigenvalue $n-1$, and the $(n-1)$-dimensional subspace whose coordinate sum is zero has eigenvalue $-1$, since $(M\mathbf x)_i=\sum_jx_j-x_i$. **The spectrum consists of one collective mode and $n-1$ zero-sum modes.**

## ↑ Ancestors (10)

1. [7B](../7b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
