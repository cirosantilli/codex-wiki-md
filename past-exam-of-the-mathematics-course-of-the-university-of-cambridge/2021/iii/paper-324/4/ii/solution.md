<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For the first output qubit,

$$
\Pr(0)=\frac12\left[1+
\langle\psi_0|C^\dagger Z_1C|\psi_0\rangle\right].
$$

A [Clifford circuit](../../../../../../clifford-circuit.md) maps the Pauli observable $Z_1$ under conjugation to a tensor-product Pauli operator $\pm P_1\otimes\cdots\otimes P_n$, found by propagating it backward through the circuit in polynomial time. Since the input is a product state,

$$
\langle\psi_0|C^\dagger Z_1C|\psi_0\rangle
=\pm\prod_j\langle\alpha_j|P_j|\alpha_j\rangle.
$$

Each factor is efficiently computable, so both one-bit output probabilities are strongly simulatable. This is [Heisenberg propagation of a Pauli observable through a Clifford circuit](../../../../../../heisenberg-propagation-of-a-pauli-observable-through-a-clifford-circuit.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 324](../../../paper-324-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
