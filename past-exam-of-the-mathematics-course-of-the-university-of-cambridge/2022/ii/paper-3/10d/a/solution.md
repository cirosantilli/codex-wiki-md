<h1 id="10d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the available unitaries to prepare

$$
|s\rangle=\frac1{\sqrt N}\sum_{i\in\mathbb Z_N}|i\rangle
$$

in the first register and

$$
|-\rangle=\frac{|0\rangle-|1\rangle}{\sqrt2}
$$

in the answer qubit. The [quantum phase kickback](../../../../../../phase-kickback.md) identity gives

$$
O_x|s\rangle|-\rangle
=\frac1{\sqrt N}\sum_i(-1)^{x_i}|i\rangle|-\rangle.
$$

Choose a unitary $F$ with $F|0\rangle=|s\rangle$, apply $F^{-1}$ to the first register, and measure it. Its amplitude at $|0\rangle$ is

$$
\langle s|
\frac1{\sqrt N}\sum_i(-1)^{x_i}|i\rangle
=\frac1N\sum_i(-1)^{x_i}.
$$

This equals $+1$ or $-1$ for a constant string and zero for a balanced string. Thus outcome $0$ means constant, while every other outcome means balanced, with certainty after one oracle query. This is the [Deutsch-Jozsa test with an arbitrary uniform-state unitary](../../../../../../deutsch-jozsa-test-with-an-arbitrary-uniform-state-unitary.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [10D](../../10d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
