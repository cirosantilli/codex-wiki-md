# Hadamard-conjugated linear oracle

↑ **Parent:** [Bernstein-Vazirani algorithm](bernstein-vazirani-algorithm.md)

Let $U_a|x\rangle|b\rangle=|x\rangle|b\oplus(a\cdot x)\rangle$ be the [Boolean quantum oracle](boolean-quantum-oracle.md) for a [linear Boolean function](linear-boolean-function.md), and put $W=H^{\otimes(n+1)}$. The [CNOT gates](controlled-not-gate.md) $C_{j\to y}^{a_j}$ implement $U_a$, where the data wires control the [ancilla qubit](ancilla-qubit.md). [CNOT control reversal in the Hadamard basis](cnot-control-reversal-in-the-hadamard-basis.md) and $W^2=I$ imply the exact [unitary operator](unitary-operator.md) identity

$$
WU_aW=\prod_{j=1}^{n}C_{y\to j}^{a_j},
\qquad
WU_aW|x\rangle|b\rangle=|x\oplus ba\rangle|b\rangle.
$$

Here $\oplus$ on strings is [bitwise exclusive or](exclusive-or.md). To conjugate a product, insert $W^2=I$ between its factors; each factor reverses its control and target, and the unused [Hadamard gates](hadamard-gate.md) cancel. The [global phase](global-phase.md) is exactly $1$. In particular, the identity holds on arbitrary [quantum superpositions](quantum-superposition.md), not only on the initialized inputs of the [Bernstein-Vazirani algorithm](bernstein-vazirani-algorithm.md).

## ↑ Ancestors (5)

1. [Bernstein-Vazirani algorithm](bernstein-vazirani-algorithm.md)
2. [Quantum algorithm](quantum-algorithm.md)
3. [Algorithm](algorithm-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Ancilla preparation for the Bernstein-Vazirani algorithm](ancilla-preparation-for-the-bernstein-vazirani-algorithm.md)
- [Bernstein-Vazirani algorithm](bernstein-vazirani-algorithm.md)
- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2010/6/3/solution.md)
