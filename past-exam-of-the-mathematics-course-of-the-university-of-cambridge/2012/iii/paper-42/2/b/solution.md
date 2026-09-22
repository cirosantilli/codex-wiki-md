<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

If $x_1,x_2$ are integral, the derived surplus and slacks

$$
x_3=2x_1+x_2-6,\qquad x_4=x_2-2x_1,\qquad x_5=8-x_1-2x_2
$$

are also nonnegative integers. Therefore an all-integer [Gomory fractional cut](../../../../../../gomory-fractional-cut.md) can be taken from the final tableau's slack row

$$
x_4+\frac53x_3+\frac43x_5=\frac23.
$$

For a nonnegative integer dictionary row $x_B+\sum_j a_jx_j=b$, the quantity $x_B+\sum_j\lfloor a_j\rfloor x_j$ is an integer at most $b$, so it is at most $\lfloor b\rfloor$. Subtracting from the row proves the cut $\sum_j\{a_j\}x_j\geq\{b\}$. Applying it here gives

$$
\boxed{2x_3+x_5\geq2.}
$$

But the original row and $x_4\geq0$ give $5x_3+4x_5\leq2$. Nonnegativity then gives

$$
2x_3+x_5\leq\frac25(5x_3+4x_5)\leq\frac45<2.
$$

This contradicts the valid cut. Therefore **the integer program is infeasible**, certified by one [Gomory fractional cut](../../../../../../gomory-fractional-cut.md). It is essential to use the PDF's constraint: the altered TeX problem would have feasible integer points.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 42](../../../paper-42-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
