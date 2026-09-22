<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Since every reduced weight is nonpositive and every feasible variable is nonnegative, any feasible assignment $x$ satisfies

$$
\sum_{i,j}c_{ij}x_{ij}
=\sum_i u_i+\sum_jv_j+\sum_{i,j}\bar c_{ij}x_{ij}
\leq\sum_i u_i+\sum_jv_j.
$$

For $x^*$, each selected entry has zero reduced weight, and each unselected entry has zero variable. Thus every product $\bar c_{ij}x^*_{ij}$ vanishes and equality holds:

$$
\boxed{c\cdot x^*=\sum_i u_i+\sum_jv_j=\max c\cdot x.}
$$

The two hypotheses therefore form one optimality certificate: the first provides a universal upper bound, and the second makes the proposed assignment attain it. This is [weak duality](../../../../weak-duality.md) plus [complementary slackness](../../../../complementary-slackness.md) for the maximization [assignment problem](../../../../assignment-problem.md). For a minimization assignment, the sign reverses: $u_i+v_j\leq c_{ij}$ gives a lower bound, with equality on the selected arcs certifying optimality.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the integer programming course of the University of Oxford](../../../split.md)
5. [Integer programming course of the University of Oxford](../../../../integer-programming-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
