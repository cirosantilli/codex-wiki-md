<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For a nearest-neighbor bond in the positive coordinate direction $\mu$, smoothness and orthogonality give

$$
\mathbf n_i\mathbin\cdot\mathbf n_{i+\hat\mu}
=-1+2|\mathbf m|^2
+\frac{a^2}{2}|\partial_\mu\widetilde{\mathbf n}|^2
+\text{higher derivatives and powers of }\mathbf m.
$$

There are two such bonds per site on the square lattice. Omitting the constant ground-state energy,

$$
S^2J\sum_{\langle ij\rangle}
\mathbf n_i\mathbin\cdot\mathbf n_j
\longrightarrow
\int d^2x\left[
\frac{JS^2}{2}|\nabla\widetilde{\mathbf n}|^2
+\frac{4JS^2}{a^2}|\mathbf m|^2
\right].
$$

The staggered part of the field coupling cancels between the two sublattices, whereas

$$
S\sum_i\mathbf B\mathbin\cdot\mathbf n_i
\longrightarrow
\frac S{a^2}\int d^2x\,
\mathbf B\mathbin\cdot\mathbf m.
$$

Including the overall minus sign of the Hamiltonian contribution to the real-time action, the continuum Lagrangian density is therefore

$$
\boxed{
\mathcal L
=\frac S{a^2}\mathbf m\mathbin\cdot
(\widetilde{\mathbf n}\times\partial_t\widetilde{\mathbf n})
-\frac{4JS^2}{a^2}|\mathbf m|^2
-\frac{JS^2}{2}|\nabla\widetilde{\mathbf n}|^2
-\frac S{a^2}\mathbf B\mathbin\cdot\mathbf m.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 337](../../../paper-337-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
