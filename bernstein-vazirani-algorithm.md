# Bernstein-Vazirani algorithm

↑ **Parent:** [Quantum algorithm](quantum-algorithm.md)

The [Bernstein-Vazirani algorithm](bernstein-vazirani-algorithm.md) identifies the coefficient string of a [linear Boolean function](linear-boolean-function.md) with one [Boolean quantum oracle](boolean-quantum-oracle.md) call. It contrasts with the $n$ calls required by the [classical query complexity of linear Boolean function identification](classical-query-complexity-of-linear-boolean-function-identification.md). Prepare the data [qubits](qubit.md) at $|0\rangle^{\otimes n}$ and an [ancilla qubit](ancilla-qubit.md) at $|1\rangle$, apply a [Hadamard gate](hadamard-gate.md) to every wire, query the [function oracle](function-oracle.md), and apply the [Hadamard gates](hadamard-gate.md) again. The full output is $|a\rangle|1\rangle$.

The mechanism is [Bernstein-Vazirani phase kickback](bernstein-vazirani-phase-kickback.md). The [Pauli X gate](pauli-x-gate.md) has [eigenvector](eigenvector.md) $|-\rangle=(|0\rangle-|1\rangle)/\sqrt2$ with [eigenvalue](eigenvalue.md) $-1$. Thus the target flips become relative [quantum phases](quantum-phase.md) on the data, giving

$$
2^{-n/2}\sum_x(-1)^{a\cdot x}|x\rangle
=\bigotimes_{j=1}^{n}\frac{|0\rangle+(-1)^{a_j}|1\rangle}{\sqrt2}.
$$

The final [Hadamard transform](hadamard-transform.md) maps this product to $|a\rangle$, so [computational-basis measurement](quantum-measurement-in-the-computational-basis.md) recovers every coefficient with certainty. The [ancilla preparation for the Bernstein-Vazirani algorithm](ancilla-preparation-for-the-bernstein-vazirani-algorithm.md) ensures the required minus sign, and the [Hadamard-conjugated linear oracle](hadamard-conjugated-linear-oracle.md) gives an exact [quantum circuit](quantum-circuit-split.md) interpretation. One query is optimal for $n\ge1$, since without a query the output cannot depend on the unknown string.

**Table of contents**

- [Ancilla preparation for the Bernstein-Vazirani algorithm](ancilla-preparation-for-the-bernstein-vazirani-algorithm.md)
- [Hadamard-conjugated linear oracle](hadamard-conjugated-linear-oracle.md)

## ↑ Ancestors (4)

1. [Quantum algorithm](quantum-algorithm.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Ancilla preparation for the Bernstein-Vazirani algorithm](ancilla-preparation-for-the-bernstein-vazirani-algorithm.md)
- [Bernstein-Vazirani algorithm](bernstein-vazirani-algorithm.md)
- [Hadamard-conjugated linear oracle](hadamard-conjugated-linear-oracle.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2019/quantum-information/3/f/solution.md)
- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2010/6/2/solution.md)
- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2010/6/3/solution.md)
