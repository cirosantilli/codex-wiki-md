<h1 id="33b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $|J,J\rangle$, tracing out subsystem 2 gives the [reduced density matrix](../../../../../../reduced-density-matrix.md)

$$
\rho_1=|j_1,j_1\rangle\langle j_1,j_1|,
$$

which is pure, so its [entanglement entropy](../../../../../../entanglement-entropy.md) is zero.

For $|J,J-1\rangle$, the two subsystem-2 factors in part (iii) are orthogonal. The partial trace therefore removes the cross terms and gives

$$
\rho_1=
\frac{j_1}{J}|j_1,j_1-1\rangle\langle j_1,j_1-1|
+\frac{j_2}{J}|j_1,j_1\rangle\langle j_1,j_1|.
$$

Its nonzero [eigenvalues](../../../../../../eigenvalue.md) are $j_1/J$ and $j_2/J$, so the [Von Neumann entropy](../../../../../../von-neumann-entropy-split.md) is

$$
S=-\frac{j_1}{J}\log\frac{j_1}{J}
-\frac{j_2}{J}\log\frac{j_2}{J}.
$$

When $j_1=j_2$, both eigenvalues are $1/2$ and $S=\log2$, the maximal entropy for a rank-two reduced state.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [33B](../../33b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
