<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Work with bounded [self-adjoint operators](../../../../../../self-adjoint-operator.md) on separable infinite-dimensional [Hilbert spaces](../../../../../../hilbert-space-split.md), the setting in which the classification holds. If $UTU^*-S$ is compact for a unitary $U$, their images in the [Calkin algebra](../../../../../../calkin-algebra.md) have identical spectra, by compact perturbation invariance and unitary conjugation. Thus their essential spectra coincide.

Conversely apply the [Weyl-von Neumann theorem](../../../../../../weyl-von-neumann-theorem.md) to write $T=D_a+K_a$ and $S=D_b+K_b$ in [orthonormal bases](../../../../../../orthonormal-basis.md), with bounded real diagonal sequences and compact errors. The essential spectrum of a diagonal operator is exactly its sequence cluster set. Indeed outside that cluster set all but finitely many entries stay a positive distance from $\lambda$, so the diagonal has an inverse on a finite-codimensional subspace and is [Fredholm](../../../../../../fredholm-operator.md). At a cluster point, infinitely many distinct basis vectors have $(D-\lambda)e_j\to0$; these are weakly null unit vectors, contradicting any [Fredholm](../../../../../../fredholm-operator.md) parametrix. This also handles a value with infinite multiplicity.

The two diagonal sequences therefore have the same cluster set. Part (c) provides permutations with $a_{m_k}-b_{n_k}\to0$. Send the $m_k$th basis vector for $T$ to the $n_k$th basis vector for $S$. Under this unitary, the diagonal difference has entries tending to zero and is compact, by finite-rank truncation. Adding the two conjugated compact errors gives **$\boxed{UTU^*-S\text{ compact}}$**.

Without separability, equality of essential spectra need not suffice, even on the same [Hilbert space](../../../../../../hilbert-space-split.md). Let $H$ have uncountable dimension and let $T,S$ be projections with infinite-dimensional kernels, but with range dimensions respectively countable and uncountable. Both essential spectra are $\{0,1\}$. After any unitary conjugation the range of $T$ is still separable. If its difference from $S$ were compact, the range of $S$ would lie in the sum of that separable range and the separable closure of the compact error's range, which is impossible. Finite-dimensional spaces also need a separate dimension convention, since essential spectra are then empty. These are genuine qualifications to a statement made without the standard separable infinite-dimensional setting.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [5](../../5.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
