<h1 id="t/t2/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Try the dual intersection $3y_1+2y_2=6$, $y_1+4y_2=4$. It gives $y=(8/5,3/5)$; the remaining constraint is $5y_1+y_2=43/5\ge5$, so it is dual feasible. Its strictly positive slack in the first column suggests $x_1=0$, while positivity of both $y$ entries suggests $Ax=b$. Solving $3x_2+x_3=1$, $2x_2+4x_3=2$ gives $x=(0,1/5,2/5)$, which is primal feasible.

Their objective values agree:

$$
\boxed{x_*=(0,1/5,2/5)^T,\quad y_*=(8/5,3/5)^T,\quad c^Tx_*=b^Ty_*=14/5.}
$$

[Weak duality](../../../../../../weak-duality.md) certifies that both are optimal. The strict first-column dual slack and the two active primal equations also show uniqueness of the primal optimum; positivity of $x_2,x_3$ forces the two dual equations, so the dual optimum is unique as well.

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [T2](../../../t2.md)
4. [T](../../../../t.md)
5. [2010](../../../../../2010-split.md)
6. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../../split.md)
7. [Probability, statistics and options II course of the University of Oxford](../../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Mathematics and statistics course of the University of Oxford](../../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
