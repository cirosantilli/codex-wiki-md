<h1 id="u/1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

If the starting length is $L=b-a$, then after $k$ interval halvings the current midpoint is at most $L/2^{k+1}$ from some root remaining in the bracket. Thus, with the midpoint returned after those halvings, it suffices to take

$$
\boxed{k\geq\max\left(0,\left\lceil\log_2\frac{L}{2\epsilon}\right\rceil\right).}
$$

If iterations instead count midpoint evaluations starting with the initial midpoint as evaluation one, the usual bound is $n\geq\lceil\log_2(L/\epsilon)\rceil$, with at least one evaluation unless an endpoint root has already been found. Stating the counting convention avoids an apparent one-step discrepancy.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [U](../../../../u.md)
5. [2011](../../../../../2011-split.md)
6. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../../../split.md)
7. [Probability, statistics and options I course of the University of Oxford](../../../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Mathematics and statistics course of the University of Oxford](../../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
