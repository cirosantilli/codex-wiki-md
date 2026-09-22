<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Diagonalize the [reduced density matrix](../../../../../../reduced-density-matrix.md) on Alice's [Hilbert space](../../../../../../hilbert-space-split.md):

$$
\rho_A=\sum_{j=1}^r\lambda_j|a_j\rangle\langle a_j|,
\qquad\lambda_j>0.
$$

For every positive [eigenvalue](../../../../../../eigenvalue.md), define a vector on Bob's [Hilbert space](../../../../../../hilbert-space-split.md) by

$$
|b_j\rangle=\lambda_j^{-1/2}(\langle a_j|\otimes I_B)|\Psi_{AB}\rangle.
$$

The definition of the [partial trace](../../../../../../partial-trace.md) gives

$$
\langle b_i|b_j\rangle
=\frac{\langle a_j|\rho_A|a_i\rangle}{\sqrt{\lambda_i\lambda_j}}
=\delta_{ij}.
$$

Thus the $|b_j\rangle$ are [orthonormal](../../../../../../orthonormal-set.md). Extend the $|a_j\rangle$ to an [orthonormal basis](../../../../../../orthonormal-basis.md) of Alice's [Hilbert space](../../../../../../hilbert-space-split.md). If $|a\rangle$ lies in the zero-[eigenvalue](../../../../../../eigenvalue.md) subspace of $\rho_A$, then

$$
\| (\langle a|\otimes I_B)|\Psi_{AB}\rangle\|^2
=\langle a|\rho_A|a\rangle=0.
$$

There is therefore no component of $|\Psi_{AB}\rangle$ in those additional basis directions. Expansion in Alice's [orthonormal basis](../../../../../../orthonormal-basis.md) yields the [Schmidt decomposition](../../../../../../schmidt-decomposition.md)

$$
\boxed{|\Psi_{AB}\rangle=\sum_{j=1}^r\sqrt{\lambda_j}|a_j\rangle|b_j\rangle,
\quad\sum_j\lambda_j=1.}
$$

Its positive [Schmidt coefficients](../../../../../../schmidt-coefficient.md) are $s_j=\sqrt{\lambda_j}$ and its [Schmidt rank](../../../../../../schmidt-rank.md) is $r$. Taking the two [partial traces](../../../../../../partial-trace.md) and using the [orthonormality](../../../../../../orthonormal-set.md) of both families gives

$$
\rho_A=\sum_j\lambda_j|a_j\rangle\langle a_j|,
\qquad
\rho_B=\sum_j\lambda_j|b_j\rangle\langle b_j|.
$$

Hence **the two reduced density matrices have exactly the same nonzero eigenvalues, including multiplicities**. Their numbers of zero [eigenvalues](../../../../../../eigenvalue.md) may differ when the local [Hilbert spaces](../../../../../../hilbert-space-split.md) have different dimensions. In particular their [Von Neumann entropies](../../../../../../von-neumann-entropy-split.md) agree.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
