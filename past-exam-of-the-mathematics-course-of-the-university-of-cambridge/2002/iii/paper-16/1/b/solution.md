<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take $\phi$ in the [identity component](../../../../../../identity-component.md) $\operatorname{Symp}_0(M,\omega)$ and choose a smooth [symplectic isotopy](../../../../../../symplectic-isotopy.md) $\phi_t$ from the identity to $\phi$. Let its generating [vector field](../../../../../../vector-field.md) be $X_t=\dot\phi_t\circ\phi_t^{-1}$. Differentiating $\phi_t^*\omega=\omega$ gives

$$
0=\phi_t^*\mathcal L_{X_t}\omega=\phi_t^*d(\iota_{X_t}\omega).
$$

Thus $\eta_t=\iota_{X_t}\omega$ is a [closed differential one-form](../../../../../../closed-differential-one-form.md). By the vanishing of the first [de Rham cohomology](../../../../../../de-rham-cohomology.md), it is exact, so choose $H_t$ with $\eta_t=-dH_t$.

The primitives can be chosen smoothly in both $t$ and the point. On each connected component fix a base point $x_0$ and define $H_t(x)=-\int_{x_0}^x\eta_t$. Exactness makes this independent of the chosen path. In a coordinate neighbourhood of any point, use a fixed path to the neighbourhood's centre followed by a smoothly varying short path; this shows smooth dependence locally, and hence globally. One may subtract a time-dependent mean without changing the [Hamiltonian vector field](../../../../../../hamiltonian-vector-field.md). Therefore the original [symplectic isotopy](../../../../../../symplectic-isotopy.md) is Hamiltonian, and $\phi\in\operatorname{Ham}(M,\omega)$.

Here the usual description of $\operatorname{Symp}_0$ by smooth isotopies agrees with the topological [identity component](../../../../../../identity-component.md). To see the local path-connectedness behind that description, use a [Weinstein neighborhood](../../../../../../weinstein-neighborhood-theorem.md) of the diagonal in $(M\times M,-\omega\oplus\omega)$. The graph of a symplectomorphism close to the identity corresponds to the graph of a small closed one-form on the diagonal. Multiplying that one-form by $t\in[0,1]$ gives Lagrangian graphs; for sufficiently small forms their first projections remain diffeomorphisms, so they give symplectomorphisms connecting the original map to the identity. These local paths, translated in the group and concatenated with smooth time reparametrizations, identify its connected and smooth-path components.

Conversely every [Hamiltonian isotopy](../../../../../../hamiltonian-isotopy.md) is symplectic by part (a), and connects its time-one map to the identity. Hence

$$
\boxed{\operatorname{Symp}_0(M,\omega)=\operatorname{Ham}(M,\omega)}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
