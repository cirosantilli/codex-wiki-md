<h1 id="t/1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the primal equality-form [linear program](../../../../../linear-programming-split.md), the [dual linear program](../../../../../dual-linear-program.md) is

$$
\boxed{\text{minimize }b^Ty\quad\text{subject to }A^Ty\geq c,\quad y\text{ unrestricted in sign}.}
$$

If $x\geq0$ is primal feasible and $y$ dual feasible, then

$$
c^Tx\leq (A^Ty)^Tx=y^TAx=b^Ty.
$$

This proves [weak duality](../../../../../weak-duality.md). Their objective gap is $\sum_j x_j((A^Ty)_j-c_j)$, a sum of nonnegative terms. The [complementary slackness](../../../../../complementary-slackness.md) theorem states that a feasible pair is optimal for the two programmes exactly when

$$
\boxed{x_j((A^Ty)_j-c_j)=0\quad\text{for every }j.}
$$

These conditions make the gap zero, which by weak duality certifies optimality; necessity follows from [strong duality](../../../../../strong-duality.md).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [1](../../1.md)
3. [T](../../../t.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options I course of the University of Oxford](../../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
