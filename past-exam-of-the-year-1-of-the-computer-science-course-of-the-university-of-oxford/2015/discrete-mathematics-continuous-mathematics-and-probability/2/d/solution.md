<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

We prove [Cassini's identity](../../../../../cassini-s-identity.md) by [mathematical induction](../../../../../mathematical-induction.md). At $n=1$,

$$
F_0F_2-F_1^2=0\cdot1-1=-1=(-1)^1.
$$

Suppose $D_n=F_{n-1}F_{n+1}-F_n^2=(-1)^n$. The [Fibonacci recurrence](../../../../../fibonacci-recurrence.md) gives $F_{n-1}=F_{n+1}-F_n$ and hence

$$
\begin{aligned}
D_{n+1}
&=F_nF_{n+2}-F_{n+1}^2\\
&=F_n(F_{n+1}+F_n)-F_{n+1}^2\\
&=-\bigl((F_{n+1}-F_n)F_{n+1}-F_n^2\bigr)
=-D_n=(-1)^{n+1}.
\end{aligned}
$$

The induction proves

$$
\boxed{F_{n-1}F_{n+1}-F_n^2=(-1)^n\qquad(n\ge1).}
$$

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [Discrete mathematics, continuous mathematics, and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
