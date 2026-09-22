<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use [superdense coding](../../../../../../superdense-coding.md). For the two-bit message $(a,b)\in\{0,1\}^2$, Alice applies $Z^aX^b$ to her half of the shared [Bell state](../../../../../../bell-state-split.md), where $X,Z$ are the [Pauli X gate](../../../../../../pauli-x-gate.md) and [Pauli Z gate](../../../../../../pauli-z-gate.md). The encoded states are

$$
\begin{array}{c|c}
(a,b)&(Z^aX^b\otimes I)|\Phi^+\rangle\\\hline
(0,0)&(|00\rangle+|11\rangle)/\sqrt2\\
(0,1)&(|01\rangle+|10\rangle)/\sqrt2\\
(1,0)&(|00\rangle-|11\rangle)/\sqrt2\\
(1,1)&(|01\rangle-|10\rangle)/\sqrt2.
\end{array}
$$

These four [Bell states](../../../../../../bell-state-split.md) are orthonormal. Alice then transmits her one [qubit](../../../../../../qubit.md) to Bob, who now holds both [qubits](../../../../../../qubit.md). A [Bell-basis measurement](../../../../../../bell-basis-measurement.md) identifies the message with probability one.

More explicitly, Bob can apply a [CNOT gate](../../../../../../controlled-not-gate.md) with the received [qubit](../../../../../../qubit.md) as control and his original [qubit](../../../../../../qubit.md) as target, followed by a [Hadamard gate](../../../../../../hadamard-gate.md) on the control. The [CNOT gate](../../../../../../controlled-not-gate.md) sends the encoded state to

$$
\frac{|0\rangle+(-1)^a|1\rangle}{\sqrt2}\otimes|b\rangle,
$$

and the [Hadamard gate](../../../../../../hadamard-gate.md) sends this to $|a\rangle\otimes|b\rangle$. Computational-basis [projective measurements](../../../../../../projective-measurement.md) therefore read out $a,b$ exactly. **One transmitted qubit, assisted by one previously shared Bell pair, communicates two classical bits.**

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
