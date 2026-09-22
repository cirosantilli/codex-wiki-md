<h1 id="17f/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Proceed by induction on $\dim V$. The zero-dimensional case has the empty [orthonormal basis](../../../../../../orthonormal-basis.md). In positive dimension, the [fundamental theorem of algebra](../../../../../../fundamental-theorem-of-algebra.md) gives a root of the [characteristic polynomial](../../../../../../characteristic-polynomial.md), hence a unit [eigenvector](../../../../../../eigenvector.md) $e$ of $\alpha$, say with [eigenvalue](../../../../../../eigenvalue.md) $\lambda$. Part (ii) makes it an [eigenvector](../../../../../../eigenvector.md) of $\alpha^*$ as well. Thus the line spanned by $e$ and its [orthogonal complement](../../../../../../orthogonal-complement.md) are invariant under both operators by the introductory adjoint argument.

On $\{e\}^\perp$, the restriction of $\alpha^*$ is the adjoint of the restriction of $\alpha$, and the restrictions still commute. The restricted [linear operator](../../../../../../linear-operator.md) is therefore normal. By induction it has an [orthonormal basis](../../../../../../orthonormal-basis.md) of [eigenvectors](../../../../../../eigenvector.md). Adjoining $e$ proves **an orthonormal eigenbasis exists for $V$**, establishing the finite-dimensional [spectral theorem](../../../../../../spectral-theorem.md) by construction.

For the final deduction, use this [orthonormal basis](../../../../../../orthonormal-basis.md) $e_j$ and write $\alpha e_j=\lambda_je_j$. Define

$$
\beta e_j=|\lambda_j|e_j,\qquad \gamma e_j=\begin{cases}(\lambda_j/|\lambda_j|)e_j,&\lambda_j\ne0,\\e_j,&\lambda_j=0.\end{cases}
$$

The real nonnegative diagonal entries make $\beta$ a [Hermitian operator](../../../../../../hermitian-operator.md), and the modulus-one diagonal entries make $\gamma$ a [unitary operator](../../../../../../unitary-operator.md). Both are diagonal in the same [orthonormal basis](../../../../../../orthonormal-basis.md), so they commute and $\beta\gamma e_j=\lambda_je_j$ even when $\lambda_j=0$. This proves the required factorization without assuming invertibility.

Conversely, if $\alpha=\beta\gamma$ with $\beta^*=\beta$, $\gamma^*\gamma=\gamma\gamma^*=I$, and $\beta\gamma=\gamma\beta$, then $\alpha^*=\gamma^*\beta$ and

$$
\alpha\alpha^*=\beta^2,\qquad \alpha^*\alpha=\gamma^*\beta^2\gamma=\beta^2.
$$

Thus $\alpha$ is normal. **Normality is equivalent to a commuting Hermitian–unitary factorization**, with the Hermitian factor even selectable nonnegative. This is the [polar decomposition](../../../../../../polar-decomposition.md) with a unitary extension on the kernel.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [17F](../../17f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
