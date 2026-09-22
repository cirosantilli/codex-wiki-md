<h1 id="2/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Induct on $n$, with the claim quantified over every $m\ge n$. At $n=0$,

$$
F_mF_1-F_0F_{m+1}=F_m=(-1)^0F_m.
$$

Suppose the identity holds for a fixed $n$ and every $m\ge n$. For $m\ge n+1$, the [Fibonacci recurrence](../../../../../../fibonacci-recurrence.md) gives

$$
\begin{aligned}
F_mF_{n+2}-F_{n+1}F_{m+1}
&=F_m(F_{n+1}+F_n)-F_{n+1}(F_m+F_{m-1})\\
&=-\big(F_{m-1}F_{n+1}-F_nF_m\big)\\
&=-(-1)^nF_{m-1-n}=(-1)^{n+1}F_{m-(n+1)}.
\end{aligned}
$$

Applying the [induction hypothesis](../../../../../../induction-hypothesis.md) with $m-1\ge n$ is legitimate. This proves **$F_mF_{n+1}-F_nF_{m+1}=(-1)^nF_{m-n}$** throughout its domain, a case of the [Fibonacci determinant identity](../../../../../../fibonacci-determinant-identity.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
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
