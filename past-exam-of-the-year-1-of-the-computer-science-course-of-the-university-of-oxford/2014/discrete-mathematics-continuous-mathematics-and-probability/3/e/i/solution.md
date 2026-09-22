<h1 id="3/e/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The printed fractional arguments require a size convention. To make the [recurrence relation](../../../../../../recurrence-relation.md) precise on positive [integers](../../../../../../integer-split.md), take a bounded base case $T(1)=t>0$ and use $m=\lceil n/4\rceil$, $n-m$ for $n\geq2$. This [integer rounding in a divide-and-conquer recurrence](../../../../../../integer-rounding-in-a-divide-and-conquer-recurrence.md) gives $1/4\leq m/n\leq1/2$. The unrounded calculation is the special split fraction $1/4$.

Prove $T(n)\leq A n\log_2n+B n$ by [strong induction](../../../../../../strong-induction.md). Put $h_0=H_2(1/4)>0$, choose $A\geq1/h_0$, and choose $B\geq t$. The base case follows. The [entropy potential for a divide-and-conquer recurrence](../../../../../../entropy-potential-for-a-divide-and-conquer-recurrence.md) gives

$$
\begin{aligned}
T(n)
&\leq A\{m\log_2m+(n-m)\log_2(n-m)\}+Bn+n\\
&=A n\log_2n+Bn+n\{1-AH_2(m/n)\}\\
&\leq A n\log_2n+Bn.
\end{aligned}
$$

The last step uses $H_2(m/n)\geq h_0$. This closes the [inductive hypothesis](../../../../../../induction-hypothesis.md) and proves $\boxed{T(n)=O(n\log n)}$ in [Big O notation](../../../../../../big-o-notation.md).

## ↑ Ancestors (13)

1. [I](../i.md)
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
