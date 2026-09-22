<h1 id="8a/a/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Start with the assumed [basis](../../../../../../../basis.md) of [eigenvectors](../../../../../../../eigenvector.md), grouping them by [eigenvalue](../../../../../../../eigenvalue.md). In each [eigenspace](../../../../../../../eigenspace.md), apply the [Gram-Schmidt process](../../../../../../../gram-schmidt-process.md), which replaces a linearly independent list by an orthonormal list with the same span. Every new vector stays within that [eigenspace](../../../../../../../eigenspace.md), since an [eigenspace](../../../../../../../eigenspace.md) is a vector subspace.

By part (iv), different [eigenspaces](../../../../../../../eigenspace.md) are orthogonal. The combined lists therefore form an [orthonormal basis](../../../../../../../orthonormal-basis.md) of the entire space, still consisting of [eigenvectors](../../../../../../../eigenvector.md). Let $U$ have these vectors as columns. Then $U$ is a [unitary matrix](../../../../../../../unitary-matrix.md), so

$$
\boxed{U^{-1}=U^\dagger,\qquad U^\dagger AU=\operatorname{diag}(\lambda_1,\ldots,\lambda_n).}
$$

This gives the required [unitary diagonalization of a normal matrix](../../../../../../../unitary-diagonalization-of-a-normal-matrix.md), including repeated [eigenvalues](../../../../../../../eigenvalue.md).

## ↑ Ancestors (12)

1. [V](../v.md)
2. [A](../../a.md)
3. [8A](../../../8a.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ia](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
