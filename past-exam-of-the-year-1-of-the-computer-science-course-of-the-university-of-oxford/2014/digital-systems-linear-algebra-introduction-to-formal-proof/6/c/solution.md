<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Solve two triangular [linear systems](../../../../../system-of-linear-equations.md), rather than forming an [inverse matrix](../../../../../matrix-inverse-split.md):

$$
\boxed{Ly=b\quad\text{by forward substitution},\qquad Ux=y\quad\text{by back substitution}.}
$$

For this [LU decomposition](../../../../../lu-decomposition.md), [forward substitution](../../../../../forward-substitution.md) gives $y_1=b_1$, $y_2=b_2+2y_1$ and $y_3=b_3-3y_1+y_2$. Then [back substitution](../../../../../back-substitution.md) gives

$$
x_3=-y_3,\qquad x_2=\frac{y_2-2x_3}{4},\qquad x_1=y_1-4x_2-x_3.
$$

All diagonal entries used as divisors are nonzero. The same [LU decomposition](../../../../../lu-decomposition.md) can be reused for many right-hand [vectors](../../../../../vector.md), with only these two triangular solves repeated.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [6](../../6.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2014](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
