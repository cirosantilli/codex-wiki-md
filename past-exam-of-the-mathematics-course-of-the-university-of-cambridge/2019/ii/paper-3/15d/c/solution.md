<h1 id="15d/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

One classical query at any chosen $x_0$ returns only $v=sx_0+t$. Every possible slope $s\in\mathbb Z_3$ is compatible with that answer by choosing $t=v-sx_0$, so no one-query classical algorithm can determine $s$ with certainty.

For the quantum algorithm, let $\omega=e^{2\pi i/3}$ and prepare

$$
|\xi_0\rangle|\xi_{-1}\rangle
=\frac1{\sqrt3}\sum_{x\in\mathbb Z_3}|x\rangle|\xi_2\rangle.
$$

Part (b) shows that the single query applies [quantum phase kickback](../../../../../../phase-kickback.md):

$$
U_f|\xi_0\rangle|\xi_{-1}\rangle
=\frac1{\sqrt3}\sum_x\omega^{f(x)}|x\rangle|\xi_{-1}\rangle
=\omega^t|\xi_s\rangle|\xi_{-1}\rangle.
$$

The unknown intercept contributes only a [global phase](../../../../../../global-phase.md). Applying $\operatorname{QFT}_3^{-1}$ to the first register produces $|s\rangle$, whose computational-basis measurement determines $s$ with certainty after one query.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [15D](../../15d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
