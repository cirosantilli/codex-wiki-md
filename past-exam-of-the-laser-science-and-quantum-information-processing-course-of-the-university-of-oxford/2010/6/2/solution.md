<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the [Hadamard basis](../../../../hadamard-basis.md) states $|\pm\rangle=(|0\rangle\pm|1\rangle)/\sqrt2$. The [Hadamard gate](../../../../hadamard-gate.md) satisfies $H|0\rangle=|+\rangle$, $H|1\rangle=|-\rangle$, and $H^2=I$. After the first three [Hadamard gates](../../../../hadamard-gate.md), the full [quantum state](../../../../quantum-state.md) is

$$
|\psi_1\rangle=|+\rangle|+\rangle|-\rangle
=\frac12\bigl(|00\rangle+|01\rangle+|10\rangle+|11\rangle\bigr)|-\rangle.
$$

The [Pauli X gate](../../../../pauli-x-gate.md) obeys $X|-\rangle=-|-\rangle$. Consequently the [Boolean quantum oracle](../../../../boolean-quantum-oracle.md) produces [phase kickback](../../../../phase-kickback.md):

$$
U_a|x\rangle|-\rangle=(-1)^{a\cdot x}|x\rangle|-\rangle.
$$

Factoring out the [ancilla qubit](../../../../ancilla-qubit.md), the four states immediately after the [function oracle](../../../../function-oracle.md) are

$$
\begin{aligned}
|\psi_{2,00}\rangle&=\tfrac12(|00\rangle+|01\rangle+|10\rangle+|11\rangle)|-\rangle=|++\rangle|-\rangle,\\
|\psi_{2,01}\rangle&=\tfrac12(|00\rangle-|01\rangle+|10\rangle-|11\rangle)|-\rangle=|+-\rangle|-\rangle,\\
|\psi_{2,10}\rangle&=\tfrac12(|00\rangle+|01\rangle-|10\rangle-|11\rangle)|-\rangle=|-+\rangle|-\rangle,\\
|\psi_{2,11}\rangle&=\tfrac12(|00\rangle-|01\rangle-|10\rangle+|11\rangle)|-\rangle=|--\rangle|-\rangle.
\end{aligned}
$$

The final [Hadamard gates](../../../../hadamard-gate.md) send $|+\rangle$ to $|0\rangle$ and $|-\rangle$ to $|1\rangle$. In particular, the printed [quantum circuit](../../../../quantum-circuit-split.md) includes a final [Hadamard gate](../../../../hadamard-gate.md) on the [ancilla qubit](../../../../ancilla-qubit.md) too. Its full outputs, ordered as $x_1,x_2,y$, are

$$
\boxed{
\begin{array}{c|c}
a&|\psi_{\mathrm{out}}\rangle\\\hline
00&|001\rangle\\
01&|011\rangle\\
10&|101\rangle\\
11&|111\rangle
\end{array}}
$$

Thus **one oracle call identifies $a$ with certainty**: a [computational-basis measurement](../../../../quantum-measurement-in-the-computational-basis.md) of the first two [qubits](../../../../qubit.md) returns $a_1a_2$. The [ancilla qubit](../../../../ancilla-qubit.md) returns to $|1\rangle$ and carries no additional information about $a$. The [Bernstein-Vazirani algorithm](../../../../bernstein-vazirani-algorithm.md) turns the pattern of relative [quantum phases](../../../../quantum-phase.md) into a definite [computational-basis state](../../../../computational-basis-state.md).

## ↑ Ancestors (12)

1. [2](../2.md)
2. [6](../../6-split.md)
3. [2010](../../split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
