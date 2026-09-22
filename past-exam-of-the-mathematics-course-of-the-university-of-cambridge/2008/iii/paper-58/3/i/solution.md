<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Schmidt decomposition theorem](../../../../../../schmidt-decomposition.md) says that a normalized vector in the [tensor product](../../../../../../tensor-product.md) of two finite-dimensional [Hilbert spaces](../../../../../../hilbert-space-split.md) can be written

$$
|\psi\rangle=\sum_{j=1}^r\sqrt{\lambda_j}\,|u_j\rangle\otimes|v_j\rangle,\qquad
\lambda_j>0,\quad\sum_{j=1}^r\lambda_j=1,\quad r\leq n_1,
$$

where both families are orthonormal. The numbers $\sqrt{\lambda_j}$ are its [Schmidt coefficients](../../../../../../schmidt-coefficient.md). The [Schmidt rank](../../../../../../schmidt-rank.md) $r$ and coefficients, including multiplicities, are uniquely determined by the state; the local vectors may be changed within degenerate eigenspaces and by compensating phases. Zero coefficients may be appended to make $n_1$ terms, since $n_2\geq n_1$.

For a proof, form the [reduced density matrix](../../../../../../reduced-density-matrix.md) $\rho_1=\operatorname{Tr}_2|\psi\rangle\langle\psi|$. It is a [Hermitian matrix](../../../../../../hermitian-operator.md) that is [positive semidefinite](../../../../../../positive-semidefinite-matrix.md), with [trace](../../../../../../matrix-trace.md) one. The [spectral theorem](../../../../../../spectral-theorem.md) supplies an [orthonormal basis](../../../../../../orthonormal-basis.md) $u_1,\ldots,u_{n_1}$ of [eigenvectors](../../../../../../eigenvector.md) with nonnegative [eigenvalues](../../../../../../eigenvalue.md) $\lambda_j$. Define the unnormalized relative vectors in the second [Hilbert space](../../../../../../hilbert-space-split.md) by

$$
|w_j\rangle=(\langle u_j|\otimes I)|\psi\rangle.
$$

Completeness of the first [orthonormal basis](../../../../../../orthonormal-basis.md) gives $|\psi\rangle=\sum_j|u_j\rangle|w_j\rangle$. In any [orthonormal basis](../../../../../../orthonormal-basis.md) $e_b$ of the second factor, the definition of the [partial trace](../../../../../../partial-trace.md) gives

$$
\langle w_i|w_j\rangle
=\sum_b\langle\psi|u_i,e_b\rangle\langle u_j,e_b|\psi\rangle
=\langle u_j|\rho_1|u_i\rangle
=\lambda_i\delta_{ij}.
$$

Thus a zero [eigenvalue](../../../../../../eigenvalue.md) gives $w_j=0$, and for each positive [eigenvalue](../../../../../../eigenvalue.md) the vector $v_j=w_j/\sqrt{\lambda_j}$ has unit norm. Distinct such vectors are orthogonal by the same identity. Substituting them gives the required [Schmidt decomposition](../../../../../../schmidt-decomposition.md), with at most $n_1$ nonzero terms.

Taking the other [partial trace](../../../../../../partial-trace.md) now gives

$$
\rho_1=\sum_{j=1}^r\lambda_j|u_j\rangle\langle u_j|,\qquad
\rho_2=\sum_{j=1}^r\lambda_j|v_j\rangle\langle v_j|.
$$

Therefore **the two reduced density matrices have identical nonzero eigenvalues, namely the squared Schmidt coefficients**. This also proves uniqueness of the coefficient multiset and shows that the [pure state](../../../../../../pure-state.md) is a [product state](../../../../../../product-state.md) exactly when $r=1$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
