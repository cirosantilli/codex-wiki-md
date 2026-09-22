<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Quantum de Finetti theorem](../../../../../../quantum-de-finetti-theorem.md) says that the fixed-$k$ [reduced density matrix](../../../../../../reduced-density-matrix.md) of an exchangeable $N$-particle state approaches

$$
\rho^{(k)}=\int \sigma^{\otimes k}\,d\mu(\sigma)
$$

as $N\to\infty$. Finite versions bound the [trace norm](../../../../../../trace-norm.md) error by a constant of order $d_{\rm loc}^2k/N$. On a bipartite lattice, the corresponding two-sublattice form is a mixture

$$
\rho_{AB}=\int \rho_A\otimes\rho_B\,d\mu(\rho_A,\rho_B)+o(1).
$$

This is the [mean-field ansatz from the quantum de Finetti theorem](../../../../../../mean-field-ansatz-from-the-quantum-de-finetti-theorem.md).

The bond energy is a [linear functional](../../../../../../linear-functional.md) of $\rho_{AB}$. A [convex combination](../../../../../../convex-combination.md) cannot have energy below its lowest product component, so it remains only to minimize

$$
\operatorname{Tr}\!\left[
(\rho_A\otimes\rho_B)\,
J\mathbf S_A\mathbin\cdot\mathbf S_B
\right]
=\frac J4\mathbf r_A\mathbin\cdot\mathbf r_B.
$$

The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) gives $\mathbf r_A\mathbin\cdot\mathbf r_B\geq-|\mathbf r_A||\mathbf r_B|\geq-1$, with equality for pure antiparallel vectors. This reproduces the [Néel state](../../../../../../neel-state.md) and $-J/4$ per bond found in part (a).

**Yes.** The limiting state saturates the de Finetti mean-field lower bound: the minimizing product state belongs to the allowed de Finetti mixture, and the finite-de-Finetti error tends to zero as $z\to\infty$. At finite $z$ the theorem gives only an approximation; entanglement and correlated fluctuations can lower the energy below the product-state value by corrections that vanish in the infinite-coordination limit.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 343](../../../paper-343-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
