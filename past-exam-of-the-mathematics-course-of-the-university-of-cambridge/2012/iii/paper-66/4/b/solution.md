<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In the [Hadamard basis](../../../../../../hadamard-basis.md), $X_D$ is diagonal with projectors $Q_\pm=(I\pm X_D)/2$. Rewrite the same [CNOT gate](../../../../../../controlled-not-gate.md) in the original tensor-factor order $S\otimes D$ as

$$
\boxed{U=I_S\otimes Q_+ + Z_S\otimes Q_-.}
$$

Expanding $P_0\otimes I+P_1\otimes X_D$ verifies this identity directly. Now $Z_S|+\rangle=|-\rangle$ and $Z_S|-\rangle=|+\rangle$, so $Z_S$ is $\widetilde X_S$ in the complementary basis. If $D$ is plus, the identity acts on $S$; if $D$ is minus, its sign-basis label flips. Hence $D$ is the control and $S$ the target in this basis.

Equivalently,

$$
(H\otimes H)\operatorname{CNOT}_{S\to D}(H\otimes H)
=\operatorname{CNOT}_{D\to S}.
$$

This [CNOT control reversal in the Hadamard basis](../../../../../../cnot-control-reversal-in-the-hadamard-basis.md) concerns the matrix in changed local bases, rather than a physical exchange of the two carriers.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
