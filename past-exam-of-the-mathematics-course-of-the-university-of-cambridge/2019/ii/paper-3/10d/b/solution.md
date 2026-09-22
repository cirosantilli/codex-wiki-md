<h1 id="10d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

When $k=N/4$,

$$
\sin\theta=\frac12,
\qquad \theta=\frac\pi6.
$$

One [Grover search algorithm](../../../../../../grover-s-algorithm.md) iteration therefore gives

$$
Q|\psi_0\rangle
=\sin(3\theta)|\psi_G\rangle+\cos(3\theta)|\psi_B\rangle
=|\psi_G\rangle.
$$

The selective sign change $I_G$ is implemented with one application of the [Boolean quantum oracle](../../../../../../boolean-quantum-oracle.md): prepare its answer qubit in $|-\rangle=(|0\rangle-|1\rangle)/\sqrt2$ and use [quantum phase kickback](../../../../../../phase-kickback.md), obtaining $(-1)^{f(x)}$ on each $|x\rangle$. The remaining operations $H_n$, $I_0$, and the final computational-basis measurement are independent of $f$. Measurement of $|\psi_G\rangle$ returns some $x\in G$ with probability one, so exactly one query to $U_f$ suffices.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [10D](../../10d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
