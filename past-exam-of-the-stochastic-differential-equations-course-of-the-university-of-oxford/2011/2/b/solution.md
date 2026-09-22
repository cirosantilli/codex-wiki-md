<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set $A_n=\{\sup_{s\leq t}|M_s^{(n)}|\geq2^{-(n-1)/2}\}$. Part (a) gives $\sum_n\mathbb P(A_n)<\infty$. The [Borel-Cantelli first lemma](../../../../borel-cantelli-first-lemma.md) implies that, almost surely, only finitely many $A_n$ occur. On the complementary full-probability event, all sufficiently late terms satisfy

$$
\sup_{s\leq t}|M_s^{(n)}|<2^{-(n-1)/2}.
$$

These deterministic bounds form a convergent geometric series. The finitely many earlier suprema are finite by continuity on the compact time interval. Hence

$$
\boxed{\sum_n\sup_{s\leq t}|M_s^{(n)}|<\infty\quad\text{almost surely}.}
$$

The series therefore converges absolutely and uniformly on $[0,t]$ by the [Weierstrass M-test](../../../../weierstrass-m-test.md), and its sample-path limit is continuous.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the stochastic differential equations course of the University of Oxford](../../../split.md)
5. [Stochastic differential equations course of the University of Oxford](../../../../stochastic-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
