<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The answer [qubit](../../../../../../qubit.md) enters the [Boolean quantum oracle](../../../../../../boolean-quantum-oracle.md) in $|-\rangle=(|0\rangle-|1\rangle)/\sqrt2$, because the [Pauli X gate](../../../../../../pauli-x-gate.md) followed by the [Hadamard gate](../../../../../../hadamard-gate.md) maps $|0\rangle$ to $|-\rangle$. Since $X|-\rangle=-|-\rangle$, [quantum phase kickback](../../../../../../phase-kickback.md) multiplies the $|xy\rangle$ component by $(-1)^{f(x,y)}$ and leaves the answer [qubit](../../../../../../qubit.md) unchanged. The two input [qubits](../../../../../../qubit.md) enter in the [uniform quantum superposition](../../../../../../uniform-quantum-superposition.md) $|++\rangle$. Thus

$$
\boxed{|\psi_{abcd}\rangle=\frac{(-1)^d}{2}\sum_{x,y\in\{0,1\}}(-1)^{axy+bx+cy}|xy\rangle\otimes|-\rangle.}
$$

Equivalently, using the [Controlled-Z gate](../../../../../../controlled-z-gate.md) and the [Pauli Z gate](../../../../../../pauli-z-gate.md),

$$
|\psi_{abcd}\rangle=(-1)^d\bigl[C_Z^a(Z^b\otimes Z^c)|++\rangle\bigr]\otimes|-\rangle.
$$

Here the exponent in the phase may be evaluated as an ordinary integer, since its parity agrees with the [exclusive or](../../../../../../exclusive-or.md) expression. In particular, $d$ contributes only a [global phase](../../../../../../global-phase.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 51](../../../paper-51-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
