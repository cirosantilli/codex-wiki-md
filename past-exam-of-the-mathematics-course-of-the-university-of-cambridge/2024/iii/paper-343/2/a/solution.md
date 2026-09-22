<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write the spin-one-half [Heisenberg antiferromagnet](../../../../../../heisenberg-antiferromagnet.md) as

$$
H_z=J\sum_{\langle ij\rangle}\mathbf S_i\mathbin\cdot\mathbf S_j,
\qquad J>0,
$$

on a bipartite lattice of [coordination number](../../../../../../coordination-number-of-a-lattice.md) $z$. A one-spin [density operator](../../../../../../density-matrix.md) is $\rho=(I+\mathbf r\mathbin\cdot\boldsymbol\sigma)/2$, where $\mathbf r$ is its [Bloch vector](../../../../../../bloch-vector.md) and $|\mathbf r|\leq1$. In a two-sublattice [product state](../../../../../../product-state.md),

$$
\langle\mathbf S_i\mathbin\cdot\mathbf S_j\rangle
=\frac14\mathbf r_A\mathbin\cdot\mathbf r_B.
$$

The minimum is $-1/4$, attained by pure antiparallel Bloch vectors, so the minimizing product state is a [Néel state](../../../../../../neel-state.md). In the $z\to\infty$ limit this [mean-field approximation](../../../../../../mean-field-approximation.md) becomes exact and the ground-state energy per bond is therefore

$$
e_{\rm bond}=-\frac J4.
$$

The phrase “energy density” requires a coupling convention. For the unscaled Hamiltonian above, every site belongs to $z/2$ bonds and

$$
\frac{E_0}{N}=-\frac{Jz}{8},
$$

which diverges as $z\to\infty$. With the standard [Kac normalization](../../../../../../coordination-number-of-a-lattice.md)

$$
H_z^{\rm Kac}=\frac Jz\sum_{\langle ij\rangle}\mathbf S_i\mathbin\cdot\mathbf S_j,
$$

the finite energy density is

$$
\lim_{z\to\infty}\frac{E_0}{N}=-\frac J8.
$$

If the convention divides by the spatial dimension $d=z/2$ instead, the answer is $-J/4$ per site. A Hamiltonian written with $\boldsymbol\sigma_i\mathbin\cdot\boldsymbol\sigma_j$ rather than $\mathbf S_i\mathbin\cdot\mathbf S_j$ multiplies all these energies by four.

## ↑ Ancestors (11)

1. [A](../a.md)
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
