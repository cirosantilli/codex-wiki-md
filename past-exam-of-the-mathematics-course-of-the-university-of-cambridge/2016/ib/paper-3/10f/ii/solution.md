<h1 id="10f/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

We prove the finite-dimensional [spectral theorem for normal operators](../../../../../../spectral-theorem-for-normal-operators.md) by induction on dimension. A complex [linear operator](../../../../../../linear-operator.md) has an [eigenvector](../../../../../../eigenvector.md) $v$ with eigenvalue $\lambda$, by the [fundamental theorem of algebra](../../../../../../fundamental-theorem-of-algebra.md). For a [normal operator](../../../../../../normal-operator.md) $T$, the operator $T-\lambda I$ is also normal, and

$$
\|(T-\lambda I)w\|^2=\|(T^*-\overline\lambda I)w\|^2
$$

for every $w$. Applying this to $v$ shows $T^*v=\overline\lambda v$.

Normalize $v$. Its [orthogonal complement](../../../../../../orthogonal-complement.md) $W=v^\perp$ is invariant under both $T$ and $T^*$: the [adjoint operator](../../../../../../adjoint-operator.md) identities pair $Tw$ with $v$ through $T^*v$, and $T^*w$ with $v$ through $Tv$. The restricted operator on $W$ remains normal, and its adjoint is the restriction of $T^*$. Induction supplies an [orthonormal eigenbasis](../../../../../../orthonormal-eigenbasis.md) of $W$, which together with $v$ gives one for $V$.

Conversely, in an [orthonormal basis](../../../../../../orthonormal-basis.md) of eigenvectors, $T$ is diagonal and $T^*$ is the diagonal matrix of the conjugate eigenvalues. The two diagonal operators commute. Thus **normality is equivalent to an orthonormal eigenbasis**. The zero-dimensional case is immediate.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [10F](../../10f.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
