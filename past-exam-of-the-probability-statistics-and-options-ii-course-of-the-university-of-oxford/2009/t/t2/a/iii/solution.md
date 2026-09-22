<h1 id="t/t2/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Take the dual vector $y=(8/17,45/17)^T$. Its column constraints have values $5,12,53/17,233/17$, exceeding or equaling $c=(5,12,2,5)^T$; its entries are positive. Thus it is dual feasible. The first two constraints are equalities while the last two have strictly positive slack, suggesting $x_3=x_4=0$. Solve the two primal equalities to get $x_1=5/17$, $x_2=3/17$, both positive.

The resulting feasible objectives agree:

$$
\boxed{x_*=(5/17,3/17,0,0)^T,\quad y_*=(8/17,45/17)^T,\quad\text{optimal value }61/17.}
$$

[Weak duality](../../../../../../weak-duality.md) proves optimality. Strict dual slack in columns three and four and positive dual entries force the two primal equalities, proving primal uniqueness; positive first two primal coordinates force the two [independent](../../../../../../independent-random-variables.md) dual equalities, proving dual uniqueness.

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [T2](../../../t2.md)
4. [T](../../../../t.md)
5. [2009](../../../../../2009-split.md)
6. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../../split.md)
7. [Probability, statistics and options II course of the University of Oxford](../../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Mathematics and statistics course of the University of Oxford](../../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
