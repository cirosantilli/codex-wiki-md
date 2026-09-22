<h1 id="4/b/protocol-2/solution">Solution</h1>

↑ **Parent:** [Protocol 2](../protocol-2.md)

**Impossible to implement as written: Bob is never given the basis string.** Step 7 requires him to know which incoming qubits were acted on by a [Hadamard gate](../../../../../../../hadamard-gate.md), but the announcement contains only the check positions. Since $H^{-1}=H$, knowing that a transformation is its own inverse does not identify which qubits need it.

Bob cannot recover the missing information from the qubits alone. For each encoded [Bell pair](../../../../../../../bell-pair.md), his [reduced density matrix](../../../../../../../reduced-density-matrix.md) is

$$
\operatorname{Tr}_A[(I\otimes H^b)|\Phi^+\rangle\langle\Phi^+|(I\otimes H^b)]=I/2
$$

for either $b=0$ or $b=1$. His entire received register has the same [density matrix](../../../../../../../density-matrix.md) $I/2^{2n}$ for every string $b$, so every local [measurement in quantum mechanics](../../../../../../../quantum-measurement-split.md) has statistics independent of $b$. Nor can one fixed unitary undo both possibilities: preserving $|\Phi^+\rangle$ requires that unitary to be proportional to $I$, whereas decoding $(I\otimes H)|\Phi^+\rangle$ requires it to be proportional to $H$. Supplying the missing basis announcement after receipt would repair the protocol and make it the third one, but that communication is absent from the printed sequence.

## ↑ Ancestors (12)

1. [Protocol 2](../protocol-2.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Paper 53](../../../../paper-53-split.md)
5. [Iii](../../../../split.md)
6. [2009](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
