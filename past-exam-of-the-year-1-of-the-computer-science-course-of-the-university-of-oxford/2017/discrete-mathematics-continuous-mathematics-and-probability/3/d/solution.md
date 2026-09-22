<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

A stronger exact formula makes the [induction](../../../../../mathematical-induction.md) explicit:

$$
\boxed{S_n=1+m\bigl(1+\lfloor\log_2n\rfloor\bigr),\qquad n\geq1.}
$$

For $n=1$, the recurrence gives $S_1=S_0+m=1+m$. For $n\geq2$, set $j=\lfloor n/2\rfloor$, so $1\leq j<n$. In the relevant binary interval, $\lfloor\log_2j\rfloor=\lfloor\log_2n\rfloor-1$. The [strong induction](../../../../../strong-induction.md) hypothesis gives

$$
S_n=S_j+m=1+m\bigl(1+\lfloor\log_2j\rfloor\bigr)+m
=1+m\bigl(1+\lfloor\log_2n\rfloor\bigr).
$$

For $n\geq2$, $S_n\leq1+m+m\log_2n\leq(1+2m)\log_2n$. Hence $S_n=O(\log_2n)$. This is an [integer-halving recurrence with constant toll](../../../../../integer-halving-recurrence-with-constant-toll.md); the separately defined $n=0$ case does not require evaluating $\log0$.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [Discrete mathematics, continuous mathematics and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
