<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Apply the [elementary row operation](../../../../../elementary-row-operation.md) $R_1\gets R_1-R_2$, which preserves the [determinant](../../../../../determinant.md). Expanding along the new first row gives

$$
\begin{aligned}
\det A&=\det\begin{pmatrix}2-c&0&0\\c&c&c\\8&7&c\end{pmatrix}\\
&=(2-c)\det\begin{pmatrix}c&c\\7&c\end{pmatrix}=(2-c)c(c-7).
\end{aligned}
$$

A square [matrix](../../../../../matrix.md) is an [invertible matrix](../../../../../invertible-matrix.md) exactly when its [determinant](../../../../../determinant.md) is nonzero. Therefore

$$
\boxed{c=0,\quad c=2,\quad c=7}
$$

are precisely the three values making $A$ a [singular matrix](../../../../../singular-matrix.md). They also have direct explanations: at $c=0$ the second row is zero, at $c=2$ the first two rows coincide, and at $c=7$ the last two columns coincide.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
