<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use [mathematical induction](../../../../../mathematical-induction.md) with the defining [Fibonacci recurrence](../../../../../fibonacci-recurrence.md). Both identities hold at $n=0$: their two sides are zero. If the first holds at $n$, then

$$
\sum_{i=0}^{n+1}F_i
=F_{n+2}-1+F_{n+1}=F_{n+3}-1.
$$

If the second holds at $n$, then

$$
\sum_{i=0}^{n+1}F_i^2
=F_nF_{n+1}+F_{n+1}^2
=F_{n+1}(F_n+F_{n+1})
=F_{n+1}F_{n+2}.
$$

Each [inductive hypothesis](../../../../../induction-hypothesis.md) therefore advances to $n+1$.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [Discrete mathematics, continuous mathematics and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2014](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
