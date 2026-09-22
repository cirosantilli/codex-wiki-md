<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use [Hadamard conjugation of a controlled gate](../../../../../hadamard-conjugation-of-a-controlled-gate.md) to obtain the [Controlled-Z gate](../../../../../controlled-z-gate.md):

$$
CZ=(I\otimes H)\operatorname{CNOT}_{1\to2}(I\otimes H)
=\operatorname{diag}(1,1,1,-1).
$$

Conjugating by [Pauli X gates](../../../../../pauli-x-gate.md) on both [qubits](../../../../../qubit.md) moves its negative entry from $|11\rangle$ to $|00\rangle$:

$$
(X\otimes X)CZ(X\otimes X)=I-2|00\rangle\langle00|.
$$

Finally $(H\otimes H)|00\rangle=|+\rangle|+\rangle=|e_0\rangle$, so a [two-qubit diffusion circuit](../../../../../two-qubit-diffusion-circuit.md) is

$$
\boxed{C=(H\otimes H)(X\otimes X)(I\otimes H)
\operatorname{CNOT}_{1\to2}(I\otimes H)(X\otimes X)(H\otimes H)=-W.}
$$

In temporal order, apply [Hadamard gates](../../../../../hadamard-gate.md) on both [qubits](../../../../../qubit.md), [Pauli X gates](../../../../../pauli-x-gate.md) on both, a [Hadamard gate](../../../../../hadamard-gate.md) on the second, a [controlled-NOT gate](../../../../../controlled-not-gate.md) $1\to2$, a [Hadamard gate](../../../../../hadamard-gate.md) on the second, [Pauli X gates](../../../../../pauli-x-gate.md) on both, then [Hadamard gates](../../../../../hadamard-gate.md) on both. Every gate is permitted. The overall minus sign is the allowed [global phase](../../../../../global-phase.md), so this implements the required [inversion about the mean](../../../../../inversion-about-the-mean.md) for [Grover search algorithm](../../../../../grover-s-algorithm.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Quantum information](../../../quantum-information-split.md)
4. [2022](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
