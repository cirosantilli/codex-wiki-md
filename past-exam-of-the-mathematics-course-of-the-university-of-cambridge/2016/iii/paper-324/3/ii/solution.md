<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The computational-basis projectors on the first [qubit](../../../../../../qubit.md) are

$$
\Pi_0=|0\rangle\langle0|\otimes I^{\otimes(n-1)},\qquad
\Pi_1=|1\rangle\langle1|\otimes I^{\otimes(n-1)}.
$$

The [Pauli Z gate](../../../../../../pauli-z-gate.md) acts as $+1$ on the first subspace and $-1$ on the second, so $Z_1=\Pi_0-\Pi_1$. By the [Born rule](../../../../../../born-rule.md), $p_b=\langle\psi|\Pi_b|\psi\rangle$. Therefore **the expectation determines the output probabilities**:

$$
\boxed{\langle\psi|Z_1|\psi\rangle=p_0-p_1,\qquad
p_0=\frac{1+\langle Z_1\rangle}{2},\quad p_1=\frac{1-\langle Z_1\rangle}{2}.}
$$

The normalization supplies $p_0+p_1=1$; no product-state assumption is needed for this identity.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 324](../../../paper-324-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
