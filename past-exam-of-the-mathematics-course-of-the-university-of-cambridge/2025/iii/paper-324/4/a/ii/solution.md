<h1 id="4/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Suppose output qubit $j$ is measured. Its probability of outcome zero is

$$
p_0=\frac12\left(1+
\langle\psi|C^\dagger Z_jC|\psi\rangle\right).
$$

Because $C$ is a [Clifford operation](../../../../../../../clifford-gate.md), the [Pauli group](../../../../../../../pauli-group.md) is preserved under conjugation. Propagating $Z_j$ backward through the $N=\operatorname{poly}(n)$ gates therefore produces, including its sign, a tensor-product Pauli

$$
C^\dagger Z_jC=\eta\,P_1\otimes\cdots\otimes P_n.
$$

The input is a [product state](../../../../../../../product-state.md), so the expectation factors:

$$
\langle\psi|C^\dagger Z_jC|\psi\rangle
=\eta\prod_{k=1}^n\langle\alpha_k|P_k|\alpha_k\rangle.
$$

Each one-qubit factor follows directly from the classical description of $|\alpha_k\rangle$, and conjugating a Pauli through each Clifford gate takes constant classical work. Hence $p_0$, and $p_1=1-p_0$, are computable in polynomial time. This is [Heisenberg propagation of a Pauli observable through a Clifford circuit](../../../../../../../heisenberg-propagation-of-a-pauli-observable-through-a-clifford-circuit.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Paper 324](../../../../paper-324-split.md)
5. [Iii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
