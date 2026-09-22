<h1 id="2/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For $n=0$, the difference is $F_1^2-F_0F_2=1=(-1)^0$. Define $D_n=F_{n+1}^2-F_nF_{n+2}$. The [Fibonacci recurrence](../../../../../../fibonacci-recurrence.md) gives

$$
\begin{aligned}
D_{n+1}
&=F_{n+2}^2-F_{n+1}F_{n+3}\\
&=F_{n+2}(F_{n+2}-F_{n+1})-F_{n+1}^2\\
&=F_nF_{n+2}-F_{n+1}^2=-D_n.
\end{aligned}
$$

The [inductive step](../../../../../../inductive-step.md) therefore changes $(-1)^n$ into $(-1)^{n+1}$. By [mathematical induction](../../../../../../mathematical-induction.md), **$D_n=(-1)^n$ for all $n\ge0$**, the requested form of [Cassini's identity](../../../../../../cassini-s-identity.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [D](../../d.md)
3. [2](../../../2.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
