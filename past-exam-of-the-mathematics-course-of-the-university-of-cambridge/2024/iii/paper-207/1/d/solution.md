<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use a three-state [continuous-time multi-state model](../../../../../../continuous-time-multi-state-model.md) with transient infected state $I$ and absorbing recovered and dead states $R$ and $D$. If recovery and death have constant [transition intensities](../../../../../../transition-intensity.md) $\gamma$ and $\mu$, its [Q-matrix](../../../../../../transition-rate-matrix.md) is

$$
Q=
\begin{pmatrix}
-(\gamma+\mu)&\gamma&\mu\\
0&0&0\\
0&0&0
\end{pmatrix},
$$

with state order $(I,R,D)$. This is also a [competing risks model](../../../../../../competing-risks-model.md): recovery and death are the two mutually exclusive first events.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
