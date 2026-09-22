<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use complex [inner products](../../../../../../inner-product.md) linear in the first argument throughout. The [spectral theorem for compact self-adjoint operators](../../../../../../spectral-theorem-for-compact-hermitian-operators.md) states that, for a [compact operator](../../../../../../compact-operator-split.md) $T=T^*$ on a [Hilbert space](../../../../../../hilbert-space-split.md), its nonzero spectral values are real [eigenvalues](../../../../../../eigenvalue.md), each of finite multiplicity, with no possible accumulation point except zero. Moreover,

$$
\boxed{H=\ker T\oplus\bigoplus_{\lambda\ne0}\ker(T-\lambda I),
\qquad T=\sum_{\lambda\ne0}\lambda P_\lambda,}
$$

where $P_\lambda$ are the mutually orthogonal [eigenspace](../../../../../../eigenspace.md) [projections](../../../../../../projection-linear-algebra.md). The operator series converges in [operator norm](../../../../../../operator-norm.md) when the nonzero [eigenvalues](../../../../../../eigenvalue.md) are listed in decreasing absolute value. The sum is at most countable, even if the [kernel](../../../../../../kernel-of-a-linear-map.md) is nonseparable. Zero need not be an [eigenvalue](../../../../../../eigenvalue.md).

First prove that a nonzero compact [self-adjoint operator](../../../../../../self-adjoint-operator.md) has an [eigenvalue](../../../../../../eigenvalue.md) of magnitude its [norm](../../../../../../norm.md), without assuming a spectral decomposition. Put $r=\|T\|>0$ and choose unit [vectors](../../../../../../vector.md) $\xi_n$ with $\|T\xi_n\|\to r$. Since $\|T^2\xi\|\leq r\|T\xi\|$, expansion gives

$$
\|(T^2-r^2I)\xi_n\|^2
\leq r^2\bigl(r^2-\|T\xi_n\|^2\bigr)\longrightarrow0.
$$

[Compactness](../../../../../../compact-space.md) of $T^2$ supplies a subsequence for which $T^2\xi_n$ converges; the displayed estimate then forces $\xi_n$ itself to converge to a unit [vector](../../../../../../vector.md) $\xi$ satisfying $T^2\xi=r^2\xi$. The [vectors](../../../../../../vector.md) $\xi+T\xi/r$ and $\xi-T\xi/r$ are [eigenvectors](../../../../../../eigenvector.md) for $r$ and $-r$, respectively, whenever nonzero, and they cannot both vanish. This proves the claim.

Self-adjointness gives reality of every [eigenvalue](../../../../../../eigenvalue.md) and [orthogonality](../../../../../../orthogonal-vectors.md) of [eigenspaces](../../../../../../eigenspace.md) for distinct [eigenvalues](../../../../../../eigenvalue.md). An [eigenspace](../../../../../../eigenspace.md) for $\lambda\ne0$ cannot contain an infinite orthonormal sequence: its images under $T$ would have pairwise distance $\sqrt2|\lambda|$, contradicting [compactness](../../../../../../compact-space.md). The same argument proves that there are only finitely many mutually orthogonal [eigenvectors](../../../../../../eigenvector.md) with [eigenvalues](../../../../../../eigenvalue.md) of magnitude at least any given $\varepsilon>0$. Hence all nonzero [eigenspaces](../../../../../../eigenspace.md) together have a countable [orthonormal basis](../../../../../../orthonormal-basis.md), and their [eigenvalues](../../../../../../eigenvalue.md) tend to zero if there are infinitely many.

Let $K$ be the [orthogonal complement](../../../../../../orthogonal-complement.md) of the closed span of all these [eigenspaces](../../../../../../eigenspace.md). It is invariant under $T$. If $T|_K$ were nonzero, the norm-attaining [eigenvalue](../../../../../../eigenvalue.md) argument applied to that compact [self-adjoint](../../../../../../self-adjoint-operator.md) restriction would produce another nonzero [eigenvector](../../../../../../eigenvector.md), a contradiction. Thus $K\subseteq\ker T$, and the converse inclusion follows from [orthogonality](../../../../../../orthogonal-vectors.md). This establishes the asserted decomposition. On its orthogonal summands the tail of the operator series has [norm](../../../../../../norm.md) equal to the supremum of the omitted [eigenvalue](../../../../../../eigenvalue.md) magnitudes, proving [norm](../../../../../../norm.md) convergence.

Finally, a nonzero complex number not among these [eigenvalues](../../../../../../eigenvalue.md) has positive distance from their set and from zero. Inverting $T-zI$ separately on the [eigenspaces](../../../../../../eigenspace.md) and [kernel](../../../../../../kernel-of-a-linear-map.md) therefore gives a bounded inverse. This proves that no other nonzero spectral values occur and completes the theorem.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
