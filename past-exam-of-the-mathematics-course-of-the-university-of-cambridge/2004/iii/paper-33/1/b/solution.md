<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**False: both primal and dual can be infeasible.** For example, take

$$
A=\begin{pmatrix}0&0\\0&1\end{pmatrix},
\qquad b=\binom{-1}{0},\qquad c=\binom10.
$$

The primal requires $0\leq-1$, so is infeasible. Its dual requires the first coordinate of $A^Ty$ to be at least $1$, namely $0\geq1$, and is also infeasible. An infeasible primal therefore does not force an unbounded dual. If the dual is additionally assumed feasible, [strong duality](../../../../../../strong-duality.md) rules out a finite dual optimum; a feasible [linear program](../../../../../../linear-programming.md) with finite optimal value attains it, so in that qualified case the dual is unbounded below.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
