<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Prepare an [ancilla qubit](../../../../../../../ancilla-qubit.md) in $|0\rangle$. To measure $X\otimes X$, apply a [Hadamard gate](../../../../../../../hadamard-gate.md) to each data qubit, apply a [controlled-NOT gate](../../../../../../../controlled-not-gate.md) from each data qubit to the ancilla, measure the ancilla in the [computational basis](../../../../../../../computational-basis.md), and apply a Hadamard gate to each data qubit again. The ancilla records the parity of the two rotated computational-basis bits, so outcome $0$ corresponds to eigenvalue $+1$ and outcome $1$ to eigenvalue $-1$. The data register is projected by $[I+(-1)^sX\otimes X]/2$, so its complete [post-measurement state](../../../../../../../post-measurement-state.md) is retained. For $Z\otimes X$, perform the same [ancilla-assisted Pauli measurement](../../../../../../../ancilla-assisted-pauli-measurement.md) but apply the basis-changing Hadamard gates only to the second data qubit.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 324](../../../../paper-324-split.md)
5. [Iii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
