<h1 id="2/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use [mathematical induction](../../../../../../mathematical-induction.md), starting at $n=1$. Since $F_0=0$ and $F_1=1$, the sum is $-1=(-1)^1F_0-1$.

Suppose the formula holds at $n\geq1$. Adding the next [Fibonacci number](../../../../../../fibonacci-number.md) with its sign and using the [Fibonacci recurrence](../../../../../../fibonacci-recurrence.md) gives

$$
\begin{aligned}
\sum_{k=0}^{n+1}(-1)^kF_k
&=(-1)^nF_{n-1}-1+(-1)^{n+1}F_{n+1}\\
&=(-1)^{n+1}(F_{n+1}-F_{n-1})-1\\
&=(-1)^{n+1}F_n-1.
\end{aligned}
$$

This is the required successor case. Thus

$$
\boxed{\sum_{k=0}^{n}(-1)^kF_k=(-1)^nF_{n-1}-1\quad(n\geq1)}.
$$

## ↑ Ancestors (13)

1. [I](../i.md)
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
