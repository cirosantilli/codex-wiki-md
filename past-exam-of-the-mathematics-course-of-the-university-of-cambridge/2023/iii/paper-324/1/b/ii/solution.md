<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the standard [ancilla-assisted Pauli measurement](../../../../../../../ancilla-assisted-pauli-measurement.md). To measure a Pauli $P$, reset the ancilla to $|0\rangle$, apply $H$, apply the controlled version of every nonidentity factor of $P$ with the ancilla as control, apply $H$ again, and measure the ancilla in the computational basis. The preceding calculation shows that outcome $s$ projects the data with

$$
\Pi_s(P)=\frac{I+(-1)^sP}{2}.
$$

First use this circuit with $P_1=Z\otimes I$, obtaining $s_1$. Since the measured ancilla is $|s_1\rangle$, apply the classically controlled correction $X^{s_1}$ to reset it to $|0\rangle$. Reuse it to measure $P_2=Z\otimes X$, obtaining $s_2$. All controlled Pauli gates and single-qubit corrections are [Clifford gates](../../../../../../../clifford-gate.md). Since $P_1P_2=P_2P_1$, the final data state is

$$
\boxed{
|\Psi_{\rm out}\rangle
=\frac{\Pi_{s_2}(P_2)\Pi_{s_1}(P_1)|A\rangle^{\otimes2}}
{\|\Pi_{s_2}(P_2)\Pi_{s_1}(P_1)|A\rangle^{\otimes2}\|}}.
$$

**Thus one resettable ancilla implements both measurements of the PBC without disturbing the already measured Pauli eigenvalue.**

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
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
