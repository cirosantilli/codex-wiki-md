<h1 id="15c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Hadamard gate](../../../../../../hadamard-gate.md) conjugates the [Pauli X gate](../../../../../../pauli-x-gate.md) into the [Pauli Z gate](../../../../../../pauli-z-gate.md):

$$
HXH=Z.
$$

When the control qubit is $|0\rangle$, all three circuits act as the identity on the target. When it is $|1\rangle$, the right-hand circuit acts on the target as $HXH=Z$. It therefore agrees with the [Controlled-Z gate](../../../../../../controlled-z-gate.md) on every [computational basis](../../../../../../computational-basis.md) state, proving

$$
\boxed{CZ=(I\otimes H)\operatorname{CNOT}_{12}(I\otimes H)}.
$$

Conjugating both sides by $I\otimes H$ and using $H^2=I$ immediately gives the reverse identity

$$
\boxed{\operatorname{CNOT}_{12}=(I\otimes H)CZ(I\otimes H)}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [15C](../../15c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
