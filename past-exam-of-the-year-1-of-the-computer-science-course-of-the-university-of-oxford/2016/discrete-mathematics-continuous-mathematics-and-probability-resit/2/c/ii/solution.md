<h1 id="2/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Fix $n\geq1$ and use [mathematical induction](../../../../../../mathematical-induction.md) on $m$ with two initial cases, as appropriate for the second-order [Fibonacci recurrence](../../../../../../fibonacci-recurrence.md). At $m=0$, the right side is $F_{n-1}F_0+F_nF_1=F_n$. At $m=1$, it is $F_{n-1}+F_n=F_{n+1}$.

If the identity holds at $m$ and $m+1$, then

$$
\begin{aligned}
F_{n+m+2}
&=F_{n+m+1}+F_{n+m}\\
&=F_{n-1}(F_{m+1}+F_m)+F_n(F_{m+2}+F_{m+1})\\
&=F_{n-1}F_{m+2}+F_nF_{m+3}.
\end{aligned}
$$

Hence the [induction](../../../../../../mathematical-induction.md) establishes

$$
\boxed{F_{n+m}=F_{n-1}F_m+F_nF_{m+1}\quad(n\geq1,\ m\geq0)}.
$$

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [Discrete mathematics, continuous mathematics and probability (resit)](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2016](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
