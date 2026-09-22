<h1 id="3/e/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the same [integer rounding in a divide-and-conquer recurrence](../../../../../../integer-rounding-in-a-divide-and-conquer-recurrence.md), now with root cost $n^2$. Since $1/4\leq m/n\leq1/2$,

$$
m^2+(n-m)^2\leq\frac58n^2.
$$

Choose $C\geq\max\{T(1),8/3\}$ and use [strong induction](../../../../../../strong-induction.md) with [inductive hypothesis](../../../../../../induction-hypothesis.md) $T(j)\leq Cj^2$. Both child sizes are positive and less than $n$, so

$$
T(n)\leq C\{m^2+(n-m)^2\}+n^2
\leq\left(\frac58C+1\right)n^2
\leq Cn^2.
$$

The same factor $5/8$ occurs for the exact fractional split. Therefore $\boxed{T(n)=O(n^2)}$ in [Big O notation](../../../../../../big-o-notation.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [E](../../e.md)
3. [3](../../../3.md)
4. [Discrete mathematics, continuous mathematics and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2014](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
