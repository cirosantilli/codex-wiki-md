<h1 id="t/1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The dual is

$$
\boxed{\text{minimize }b^Ty
\quad\text{subject to }A^Ty\geq c,\quad y\geq0.}
$$

[weak duality](../../../../../weak-duality.md) says that any feasible primal $x$ and dual $y$ satisfy $c^Tx\leq b^Ty$. Indeed,

$$
c^Tx\leq(A^Ty)^Tx=y^TAx\leq y^Tb.
$$

The first inequality uses $x\geq0$ and $A^Ty-c\geq0$, and the second uses $y\geq0$ and $b-Ax\geq0$. This proves the theorem. In particular, feasible solutions with equal [objective function](../../../../../objective-function.md) values are optimal for both problems.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [1](../../1.md)
3. [T](../../../t.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options I course of the University of Oxford](../../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
