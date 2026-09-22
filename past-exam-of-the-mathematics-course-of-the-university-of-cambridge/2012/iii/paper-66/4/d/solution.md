<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

To use $S$ as the apparatus, prepare it in the ready state **$|+\rangle_S$** and later read it in the [Hadamard basis](../../../../../../hadamard-basis.md). For an arbitrary input $\alpha|+\rangle_D+\beta|-\rangle_D$, part (b) gives

$$
|+\rangle_S(\alpha|+\rangle_D+\beta|-\rangle_D)
\longmapsto
\alpha|+\rangle_S|+\rangle_D+\beta|-\rangle_S|-\rangle_D.
$$

The two apparatus states are orthogonal, so its readout measures the corresponding projectors on $D$ and preserves each input [eigenstate](../../../../../../eigenstate.md). The observable is

$$
\boxed{X_D=\widetilde Z_D,}
$$

with outcomes $+1$ and $-1$. This is the [measurement direction of a CNOT interaction](../../../../../../measurement-direction-of-a-cnot-interaction.md) in the complementary basis.

The ready state and readout basis matter. Keeping $S$ in the original $|0\rangle_S$ would make the old-basis controlled gate act as the identity on $D$, producing no record. Thus the same interaction can serve either measurement direction, with different apparatus preparation and pointer readout; the [Hamiltonian operator](../../../../../../hamiltonian-quantum-mechanics.md) alone does not assign an intrinsic system/apparatus role.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
