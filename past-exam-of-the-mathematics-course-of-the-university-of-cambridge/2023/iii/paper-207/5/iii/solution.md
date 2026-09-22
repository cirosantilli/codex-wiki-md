<h1 id="5/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

At month 24 the durations and statuses are

$$
A:24\text{ censored},\quad B:7\text{ death},\quad
C:13\text{ death},\quad D:13\text{ censored},\quad
E:7\text{ death},\quad F:9\text{ censored}.
$$

At duration seven, two of six patients die, giving $2/3$. Patient F is censored at duration nine. At duration thirteen, C dies while C, D, and A are at risk; treating an event before censoring at a tied time gives a factor $2/3$. Hence

$$
\widehat F_{24}(t)=
\begin{cases}
1,&0\leq t<7,\\
\dfrac23,&7\leq t<13,\\
\dfrac49,&t\geq13.
\end{cases}
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [5](../../5.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
