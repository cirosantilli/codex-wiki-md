<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [density operator](../../../../../../density-matrix.md) is Hermitian, [positive semidefinite](../../../../../../positive-semidefinite-matrix.md) and has [trace](../../../../../../matrix-trace.md) one. Part (a) therefore makes all its coordinates real, and the identity basis vector fixes the final coordinate:

$$
\boxed{r_{N^2}=\operatorname{Tr}(\rho I/\sqrt N)=1/\sqrt N.}
$$

The remaining basis vectors are traceless by orthogonality to $I/\sqrt N$. The [Generalized Bloch representation](../../../../../../generalized-bloch-representation.md) is consequently

$$
\rho=\frac IN+\sum_{k=1}^{N^2-1}s_k\sigma_k.
$$

Using orthonormality to expand the squared [Hilbert-Schmidt norm](../../../../../../hilbert-schmidt-norm.md) gives the [purity bound for generalized Bloch vectors](../../../../../../purity-bound-for-generalized-bloch-vectors.md):

$$
\operatorname{Tr}(\rho^2)=\sum_{k=1}^{N^2}r_k^2
=\frac1N+\|s\|^2.
$$

If $p_1,\ldots,p_N$ are its nonnegative [eigenvalues](../../../../../../eigenvalue.md), then $\sum_jp_j=1$ and

$$
1-\operatorname{Tr}(\rho^2)=\left(\sum_jp_j\right)^2-\sum_jp_j^2
=2\sum_{j<k}p_jp_k\geq0.
$$

It follows that

$$
\boxed{\|s\|\leq\sqrt{1-1/N}.}
$$

Equality requires every pairwise product $p_jp_k$ to vanish, so exactly one [eigenvalue](../../../../../../eigenvalue.md) equals one and all others are zero. Conversely, a rank-one projector has precisely that [spectrum](../../../../../../spectrum-functional-analysis.md) and attains equality. Thus equality holds exactly for a [pure state](../../../../../../pure-state.md). This normalization is different from the commonly used unit-radius qubit [Bloch vector](../../../../../../bloch-vector.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 52](../../../paper-52-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
