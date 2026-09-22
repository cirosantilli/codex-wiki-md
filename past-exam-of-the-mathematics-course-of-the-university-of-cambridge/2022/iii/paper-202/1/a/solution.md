<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [L2 martingale convergence theorem](../../../../../../l2-martingale-convergence-theorem.md) gives $M_t\to M_\infty$ in $L^2$, so

$$
\|M_\infty\|_2\leq
\left\|\sup_{t\geq0}|M_t|\right\|_2.
$$

Conversely, apply the [Doob L2 maximal inequality](../../../../../../doob-l2-maximal-inequality.md) on $[0,T]$:

$$
\mathbb E\sup_{t\leq T}|M_t|^2
\leq4\mathbb E|M_T|^2
\leq4\mathbb E|M_\infty|^2.
$$

[Monotone convergence](../../../../../../monotone-convergence-theorem.md) as $T\to\infty$ gives

$$
\left\|\sup_{t\geq0}|M_t|\right\|_2
\leq2\|M_\infty\|_2.
$$

**Thus the two norms are equivalent.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
