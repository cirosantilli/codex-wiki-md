<h1 id="1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Use the unsquared convention for [quantum fidelity](../../../../../../fidelity-of-quantum-states.md):

$$
F(\tau,\omega)=\operatorname{Tr}\sqrt{\sqrt\tau\,\omega\sqrt\tau}.
$$

Choose a [purification of a density operator](../../../../../../purification-of-a-density-operator.md) $|\Psi\rangle_{RA}$ of $\rho$, and put $\tau_{RA}=(\operatorname{id}_R\otimes\Lambda)(|\Psi\rangle\langle\Psi|)$. By definition,

$$
F_e(\rho,\Lambda)=\langle\Psi|\tau_{RA}|\Psi\rangle
=F(|\Psi\rangle\langle\Psi|,\tau_{RA})^2.
$$

The [monotonicity of quantum fidelity under partial trace](../../../../../../monotonicity-of-quantum-fidelity-under-partial-trace.md) follows from [Uhlmann's theorem](../../../../../../uhlmann-s-theorem.md): maximizing purifications of two joint states are also candidate purifications of their marginals, with the discarded subsystem included in the purifying system. The optimization for the marginals therefore cannot give a smaller overlap. Here those marginals are $\rho$ and $\Lambda(\rho)$. Consequently

$$
\boxed{F_e(\rho,\Lambda)\leq F(\rho,\Lambda(\rho))^2.}
$$

This [entanglement fidelity bound by state fidelity](../../../../../../entanglement-fidelity-bound-by-state-fidelity.md) distinguishes preserving a reference entanglement from merely reproducing the input marginal.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [1](../../1.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
