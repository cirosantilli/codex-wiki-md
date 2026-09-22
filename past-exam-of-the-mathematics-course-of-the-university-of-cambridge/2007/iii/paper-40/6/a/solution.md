<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $z_i\in\{0,1\}$ indicate that item $i$ is placed in the first bin; otherwise it is placed in the second. The [two-bin load balancing](../../../../../../two-bin-load-balancing.md) problem has the familiar mixed-integer formulation

$$
\begin{gathered}
\min y,\\
\sum_iw_iz_i\leq y,\qquad\sum_iw_i(1-z_i)\leq y,\\
z_i\in\{0,1\},\qquad y\geq0.
\end{gathered}
$$

The continuous variable $y$ becomes the maximum of the two bin loads at an optimum. A pure binary [integer program](../../../../../../integer-programming.md), avoiding any integrality assumption on the weights or on $y$, is obtained by labelling a heavier bin as the first bin:

$$
\boxed{\min\sum_iw_iz_i\quad\text{subject to}\quad 2\sum_iw_iz_i\geq s,\quad z_i\in\{0,1\}.}
$$

The constraint ensures that the first load is at least the second, so the objective is their maximum. Every partition can be relabelled in this way, and every binary solution gives a partition. Thus this all-integer assignment formulation has exactly the original optimal value.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
