<h1 id="10d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let the unknown qubit be $|\alpha\rangle=a|0\rangle+b|1\rangle$. Alice holds this qubit and her half of the shared [Bell state](../../../../../../bell-state-split.md) $|\Psi^+\rangle$, while Bob holds the other half.

Alice performs a measurement of her two qubits in the Bell basis and sends the two-bit outcome to Bob through the classical channel. For the shared state $|\Psi^+\rangle$, the [teleportation with the psi-plus Bell state](../../../../../../teleportation-with-the-psi-plus-bell-state.md) correction table is

$$
\begin{array}{c|c|c}
\text{Alice's outcome}&\text{Bob's state}&\text{Bob applies}\\ \hline
\Phi^+&X|\alpha\rangle&X\\
\Phi^-&XZ|\alpha\rangle&ZX\\
\Psi^+&|\alpha\rangle&I\\
\Psi^-&Z|\alpha\rangle&Z
\end{array}
$$

up to physically irrelevant global phases. Here $X$ and $Z$ are the [Pauli X gate](../../../../../../pauli-x-gate.md) and [Pauli Z gate](../../../../../../pauli-z-gate.md). After the indicated correction, Bob's qubit is $|\alpha\rangle$. This is [quantum teleportation](../../../../../../quantum-teleportation.md); no physical copy of the unknown qubit is sent.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [10D](../../10d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
