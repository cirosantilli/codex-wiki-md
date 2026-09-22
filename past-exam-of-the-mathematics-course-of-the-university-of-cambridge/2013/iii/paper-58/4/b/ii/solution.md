<h1 id="4/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use one target [ancilla qubit](../../../../../../../ancilla-qubit.md) initially in $|0\rangle$. Apply a [CNOT gate](../../../../../../../controlled-not-gate.md) from each data [qubit](../../../../../../../qubit.md) $x_j$ to that same target, for $j=1,\ldots,n$. Each [CNOT gate](../../../../../../../controlled-not-gate.md) adds its control bit modulo two without changing the control. After all $n$ gates the target contains the [parity bit](../../../../../../../parity-bit.md) $f(x)=x_1\oplus\cdots\oplus x_n$. Thus **the required circuit is the $n$-gate parity fan-in:**

$$
\boxed{W=\prod_{j=1}^{n}\operatorname{CNOT}_{j\to a},\qquad W|x\rangle|0\rangle=|x\rangle|f(x)\rangle.}
$$

This is [parity computation by CNOT gates](../../../../../../../parity-computation-by-cnot-gates.md). The circuit also satisfies $W|x\rangle|y\rangle=|x\rangle|y\oplus f(x)\rangle$ for either target value, and $W^{-1}=W$ because all these shared-target [CNOT gates](../../../../../../../controlled-not-gate.md) commute and individually square to the identity. The action on general superpositions follows by [linearity](../../../../../../../linearity.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Paper 58](../../../../paper-58-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
