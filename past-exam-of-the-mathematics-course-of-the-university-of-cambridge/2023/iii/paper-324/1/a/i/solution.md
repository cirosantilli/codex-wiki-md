<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [strong classical simulation of a quantum circuit](../../../../../../../strong-classical-simulation-of-a-quantum-circuit.md) computes any requested output probability

$$
p(y)=\Pr(Y=y),\qquad y\in\{0,1\}^k,
$$

in [polynomial time](../../../../../../../polynomial-time.md), to the prescribed inverse-polynomial accuracy. A [weak classical simulation of a quantum circuit](../../../../../../../weak-classical-simulation-of-a-quantum-circuit.md) instead produces classical samples from the circuit's output distribution, with exact or suitably small total-variation error.

The [Extended Gottesman--Knill theorem](../../../../../../../extended-gottesman-knill-theorem.md) states that a unitary [Clifford circuit](../../../../../../../clifford-circuit.md) with an arbitrary [product state](../../../../../../../product-state.md) input and final computational-basis measurements is weakly classically simulable. It is strongly simulable when only $O(\log n)$ output qubits are measured. Indeed, each joint output projector expands into $2^k$ [Pauli operators](../../../../../../../pauli-operator.md), and Clifford conjugation maps every such operator to another Pauli operator whose expectation factors over the input qubits. The factor $2^k$ is polynomial precisely for $k=O(\log n)$.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 324](../../../../paper-324-split.md)
5. [Iii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
