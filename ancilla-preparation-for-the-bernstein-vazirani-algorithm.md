# Ancilla preparation for the Bernstein-Vazirani algorithm

↑ **Parent:** [Bernstein-Vazirani algorithm](bernstein-vazirani-algorithm.md)

The displayed [Bernstein-Vazirani algorithm](bernstein-vazirani-algorithm.md) prepares its [ancilla qubit](ancilla-qubit.md) in the [computational-basis state](computational-basis-state.md) $|1\rangle$ before the first [Hadamard gate](hadamard-gate.md). At the [function oracle](function-oracle.md) it is therefore the $-1$ [eigenstate](eigenstate.md) $|-\rangle$ of the [Pauli X gate](pauli-x-gate.md), which enables [phase kickback](phase-kickback.md). Preparing $|0\rangle$ instead yields $|+\rangle$ at the [function oracle](function-oracle.md); target flips leave this state unchanged, so the data contain no information about $a$.

The [Hadamard-conjugated linear oracle](hadamard-conjugated-linear-oracle.md) makes the more general statement transparent. With zero data and initial [ancilla qubit](ancilla-qubit.md) $\alpha|0\rangle+\beta|1\rangle$, the full fixed [quantum circuit](quantum-circuit-split.md) outputs

$$
\alpha|0\rangle^{\otimes n}|0\rangle+\beta|a\rangle|1\rangle.
$$

For nonzero $a$, the correct data outcome has [probability](probability.md) $|\beta|^2$. To obtain exact identification for all $a$, this preparation must have $\alpha=0$, so it is $|1\rangle$ up to [global phase](global-phase.md). This is a condition on the prescribed preparation circuit: any alternative [quantum state preparation](quantum-state-preparation.md) that supplies $|-\rangle$ at the [function oracle](function-oracle.md) is equivalent.

## ↑ Ancestors (5)

1. [Bernstein-Vazirani algorithm](bernstein-vazirani-algorithm.md)
2. [Quantum algorithm](quantum-algorithm.md)
3. [Algorithm](algorithm-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Bernstein-Vazirani algorithm](bernstein-vazirani-algorithm.md)
- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2010/6/3/solution.md)
