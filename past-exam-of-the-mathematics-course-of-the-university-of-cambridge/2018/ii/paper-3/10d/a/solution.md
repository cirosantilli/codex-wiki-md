<h1 id="10d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Apply a [Pauli X gate](../../../../../../pauli-x-gate.md) and then a [Hadamard gate](../../../../../../hadamard-gate.md) to the third qubit, and apply Hadamard gates to the first two. This prepares

$$
\left(\frac12\sum_{x\in B_2}|x\rangle\right)|-\rangle,
\qquad
|-\rangle=\frac{|0\rangle-|1\rangle}{\sqrt2}.
$$

One application of the [Boolean quantum oracle](../../../../../../boolean-quantum-oracle.md) now gives, by [quantum phase kickback](../../../../../../phase-kickback.md),

$$
U_f\left(\frac12\sum_x|x\rangle|-\rangle\right)
=\frac12\sum_x(-1)^{f(x)}|x\rangle|-\rangle
=|f\rangle|-\rangle.
$$

The answer qubit is unentangled and may be ignored. If all three qubits must be restored to the displayed register form, applying $H$ and then $X$ to the answer qubit maps $|-\rangle$ back to $|0\rangle$. Thus **the first register is exactly $|f\rangle$ after one use of $U_f$.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [10D](../../10d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
