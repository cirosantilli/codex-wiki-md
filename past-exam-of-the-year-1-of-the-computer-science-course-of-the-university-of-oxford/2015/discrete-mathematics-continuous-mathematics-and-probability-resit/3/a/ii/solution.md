<h1 id="3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

We prove the stronger bound $T(n)\leq2n^2$ for every $n\geq1$ by [strong induction](../../../../../../strong-induction.md). The initial case is $T(1)=1\leq2$. For $n\geq2$, put $m=\lfloor n/2\rfloor$. Then $1\leq m<n$, so the induction hypothesis and the defining [recurrence relation](../../../../../../recurrence-relation.md) give

$$
T(n)=2T(m)+n^2\leq4m^2+n^2\leq4(n/2)^2+n^2=2n^2.
$$

Thus

$$
\boxed{T(n)\leq2n^2\ (n\geq1),\qquad T(n)=O(n^2).}
$$

The [recurrence relation](../../../../../../recurrence-relation.md) must be read as applying for $n\geq2$; applying it at $n=1$ would invoke $T(0)$ outside the printed [domain](../../../../../../domain-mathematical-analysis.md). No value of $T(0)$ is needed.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Discrete mathematics, continuous mathematics, and probability (resit)](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
