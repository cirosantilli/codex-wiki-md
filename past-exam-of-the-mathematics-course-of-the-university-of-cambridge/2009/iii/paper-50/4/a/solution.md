<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

**Yes: use [superdense coding](../../../../../../superdense-coding.md), with a shared [Bell state](../../../../../../bell-state-split.md).** Let the sender and receiver initially hold the first and second [qubits](../../../../../../qubit.md) of $|\Phi^+\rangle=(|00\rangle+|11\rangle)/\sqrt2$. To encode bits $(a,b)$, the sender applies $Z^aX^b$ to her [qubit](../../../../../../qubit.md). These [Pauli operators](../../../../../../pauli-operator.md) produce four orthogonal states:

$$
\begin{array}{c|c}
(a,b)&(Z^aX^b\otimes I)|\Phi^+\rangle\\
(0,0)&(|00\rangle+|11\rangle)/\sqrt2\\
(1,0)&(|00\rangle-|11\rangle)/\sqrt2\\
(0,1)&(|01\rangle+|10\rangle)/\sqrt2\\
(1,1)&(|01\rangle-|10\rangle)/\sqrt2
\end{array}
$$

She sends this [qubit](../../../../../../qubit.md) through the noiseless [quantum channel](../../../../../../quantum-channel.md). The receiver then possesses both [qubits](../../../../../../qubit.md). He applies a [controlled-NOT gate](../../../../../../controlled-not-gate.md) from the received [qubit](../../../../../../qubit.md) to his original [qubit](../../../../../../qubit.md), followed by a [Hadamard gate](../../../../../../hadamard-gate.md) on the received [qubit](../../../../../../qubit.md). This maps the four states in the table to $|ab\rangle$. A measurement in the [computational basis](../../../../../../computational-basis.md) therefore recovers the two bits with certainty. No classical message is sent.

The resource assumption deserves care: one-qubit [superdense coding](../../../../../../superdense-coding.md) needs a [Bell pair](../../../../../../bell-pair.md) already shared before encoding. If none is initially available, the sender can prepare a [Bell pair](../../../../../../bell-pair.md) locally and send one half through the same noiseless [quantum channel](../../../../../../quantum-channel.md) in advance. The protocol then uses two transmitted [qubits](../../../../../../qubit.md) in total, including distribution of the entanglement, still with no classical communication. Alternatively, sending two [computational basis](../../../../../../computational-basis.md) [qubits](../../../../../../qubit.md) directly also communicates two bits. **With a pre-shared [Bell pair](../../../../../../bell-pair.md), one transmitted [qubit](../../../../../../qubit.md) suffices; without it, the entanglement-distribution cost must be counted.** An unassisted single transmitted [qubit](../../../../../../qubit.md) cannot perfectly encode four classical messages: its [Holevo bound](../../../../../../holevo-s-theorem.md) is at most $\log_2 2=1$ bit.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
