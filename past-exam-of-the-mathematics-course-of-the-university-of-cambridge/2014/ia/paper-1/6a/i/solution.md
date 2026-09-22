<h1 id="6a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

View a possible complex [eigenvector](../../../../../../eigenvector.md) $v$ using the [Hermitian inner product](../../../../../../hermitian-form.md). For a real [symmetric matrix](../../../../../../symmetric-matrix.md), $A^\dagger=A$, so $v^\dagger Av$ is real. Since $v^\dagger Av=\lambda v^\dagger v$ and $v^\dagger v>0$, **every [eigenvalue](../../../../../../eigenvalue.md) is real**.

For [eigenvectors](../../../../../../eigenvector.md) $v,w$ with distinct [eigenvalues](../../../../../../eigenvalue.md) $\lambda,\mu$, symmetry gives

$$
\lambda v^\dagger w=(Av)^\dagger w=v^\dagger Aw=\mu v^\dagger w,
$$

so **$v^\dagger w=0$**. In particular, real [eigenvectors](../../../../../../eigenvector.md) are [orthogonal](../../../../../../orthogonal-vectors.md) in the real [dot product](../../../../../../dot-product.md).

Use the permitted diagonalizability assumption to take bases of the real [eigenspaces](../../../../../../eigenspace.md) whose union spans $\mathbb R^n$. Apply the [Gram-Schmidt process](../../../../../../gram-schmidt-process.md) within each [eigenspace](../../../../../../eigenspace.md). Its linear combinations remain [eigenvectors](../../../../../../eigenvector.md) of that same [eigenvalue](../../../../../../eigenvalue.md); vectors in different [eigenspaces](../../../../../../eigenspace.md) are already [orthogonal](../../../../../../orthogonal-vectors.md). The resulting union is **an [orthonormal basis](../../../../../../orthonormal-basis.md) of [eigenvectors](../../../../../../eigenvector.md)**, giving an [orthogonal diagonalization of a real symmetric matrix](../../../../../../orthogonal-diagonalization-of-a-real-symmetric-matrix.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [6A](../../6a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
