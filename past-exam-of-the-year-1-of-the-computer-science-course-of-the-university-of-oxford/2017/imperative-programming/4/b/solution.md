<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $m>0$, $1/q\leq m/n$ is equivalent to $q\geq n/m$. The largest allowed [unit fraction](../../../../../unit-fraction.md) therefore has the smallest such integer denominator:

$$
\boxed{q=\left\lceil\frac nm\right\rceil.}
$$

The residual is $(mq-n)/(nq)$. From $(q-1)m<n\leq qm$ we obtain

$$
\boxed{0\leq mq-n<m.}
$$

Thus the nonnegative numerator strictly decreases at each nonfinal step, and reduction to lowest terms can only decrease it further. This [loop variant](../../../../../loop-variant.md) proves termination of the [greedy Egyptian fraction expansion](../../../../../greedy-egyptian-fraction-expansion.md). The case $m=0$ already has the empty expansion and requires no division by $m$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
