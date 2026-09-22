<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

When $a=0$, the first two [qubits](../../../../../../qubit.md) after the [Boolean quantum oracle](../../../../../../boolean-quantum-oracle.md) are $(-1)^d Z^b|+\rangle\otimes Z^c|+\rangle$. The [Hadamard gate](../../../../../../hadamard-gate.md) obeys $HZ^t|+\rangle=|t\rangle$ for $t\in\{0,1\}$. Applying the [Walsh-Hadamard transform](../../../../../../walsh-hadamard-transform.md) therefore gives

$$
(H\otimes H\otimes I)|\psi_{0bcd}\rangle=(-1)^d|bc\rangle\otimes|-\rangle.
$$

Consequently the [quantum measurement in the computational basis](../../../../../../quantum-measurement-in-the-computational-basis.md) has the deterministic outcomes

$$
\begin{array}{c|cccc}
\text{oracle}&f_{0001}&f_{0010}&f_{0100}&f_{0110}\\\hline
\text{outcome}&00&01&10&11
\end{array}
$$

These four distinct answers identify the four promised [Boolean quantum oracles](../../../../../../boolean-quantum-oracle.md) with **one query and certainty**. The constant term does not affect the [measurement in quantum mechanics](../../../../../../quantum-measurement-split.md), because a [global phase](../../../../../../global-phase.md) does not change its [probabilities](../../../../../../probability.md).

## ↑ Ancestors (11)

1. [B](../b.md)
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
