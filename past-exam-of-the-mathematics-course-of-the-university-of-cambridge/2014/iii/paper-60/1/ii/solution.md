<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

[Uhlmann's theorem](../../../../../../uhlmann-s-theorem.md) identifies [quantum fidelity](../../../../../../fidelity-of-quantum-states.md) with the largest absolute overlap of [purifications of a density operator](../../../../../../purification-of-a-density-operator.md). Choose a common reference [Hilbert space](../../../../../../hilbert-space-split.md) $R$ of dimension at least that of the original system. Then

$$
F(\rho_A,\sigma_A)=\max_{|u\rangle,|v\rangle}|\langle u|v\rangle|,
$$

where $|u\rangle,|v\rangle\in\mathcal H_A\otimes\mathcal H_R$ have reduced [density operators](../../../../../../density-matrix.md) $\rho_A,\sigma_A$. One purification may be fixed in advance: the maximum is over the other, with the freedom to apply a unitary on the reference system. This is the [unitary freedom of purification](../../../../../../unitary-freedom-of-purification.md). Enlarging the reference by unused dimensions does not change the maximum.

Take maximizing purifications $|u\rangle,|v\rangle$ of $\rho_{AB},\sigma_{AB}$ on $ABR$. Their overlap has magnitude $F(\rho_{AB},\sigma_{AB})$. Regard these same vectors as purifications of $\rho_A,\sigma_A$ with reference system $BR$. They are candidates in the larger optimization, so [Uhlmann's theorem](../../../../../../uhlmann-s-theorem.md) gives

$$
\boxed{F(\rho_A,\sigma_A)\geq F(\rho_{AB},\sigma_{AB}).}
$$

This is [monotonicity of quantum fidelity under partial trace](../../../../../../monotonicity-of-quantum-fidelity-under-partial-trace.md): discarding a system cannot make two states more distinguishable according to their [quantum fidelity](../../../../../../fidelity-of-quantum-states.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
