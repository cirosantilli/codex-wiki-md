<h1 id="1/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Propagate each output observable backwards through the [Clifford circuit](../../../../../../../clifford-circuit.md) and write

$$
Q_i=C^\dagger Z_iC.
$$

The $Q_i$ are mutually commuting [Pauli operators](../../../../../../../pauli-operator.md), and measuring them on $|0\rangle^{\otimes n}\otimes|\phi\rangle$ has exactly the required joint output distribution. Initially the first $n$ qubits are constrained by the [stabilizer generators](../../../../../../../stabilizer-generator.md) $Z_1,\ldots,Z_n$. Process the $Q_i$ in order. If $Q_i$ anticommutes with a current generator, part b gives a uniform outcome and a [Clifford operation](../../../../../../../clifford-gate.md) that replaces that generator by $Q_i$; this step needs no measurement on $|\phi\rangle$. If $Q_i$ commutes with every current generator, multiply it by known generators to remove its action on the first register. What remains is a Pauli observable $P_j$ on the $t$ resource qubits and is measured there. The nontrivial $P_j$ are independent and mutually commuting. An independent commuting family of [Pauli operators](../../../../../../../pauli-operator.md) on $t$ qubits has at most $t$ members, so $s\leq t$. All effective observables are fixed by the original commuting family; the sampled outcomes merely update the classical Clifford frame. The resulting nonadaptive [Pauli-based computation](../../../../../../../pauli-based-computation.md), followed by the stated $Z_1,\ldots,Z_n$ outputs, is therefore a [weak classical simulation of a quantum circuit](../../../../../../../weak-classical-simulation-of-a-quantum-circuit.md) with the same joint distribution.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [Paper 324](../../../../paper-324-split.md)
5. [Iii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
