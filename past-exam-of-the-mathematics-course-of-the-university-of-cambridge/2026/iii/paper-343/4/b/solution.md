<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $Z_e$ denote the dual edge variable. The PEPO implements the domain-wall map

$$
Z_uZ_v\longleftrightarrow Z_{e=(uv)},
\qquad
X_v\longleftrightarrow
A_v=\prod_{e\ni v}X_e.
$$

Because edge domain walls arise from vertex spins, their product around every plaquette is constrained:

$$
B_p=\prod_{e\in\partial p}Z_e=1.
$$

Thus the transverse-field Ising operators map to the $\mathbb Z_2$ lattice-gauge operators, while the image is projected into the positive eigenspace of all $B_p$. At the commuting-projector fixed point, adjoining these automatic projectors gives

$$
\boxed{
H_{\rm TC}
=-\sum_vA_v-\sum_pB_p},
$$

the [toric code](../../../../../../toric-code.md) Hamiltonian. Conversely, solving the zero-flux constraint writes $Z_e=Z_uZ_v$ locally and recovers the Ising variables, establishing the duality on the supported symmetry sectors.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 343](../../../paper-343-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
