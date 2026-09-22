<h1 id="27g/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $\varepsilon>0$,

$$
\begin{aligned}
\mathbb P\{M_n\leq(1-\varepsilon)\log n\}
&=\left(1-n^{-(1-\varepsilon)}\right)^n\\
&\leq\exp(-n^\varepsilon),
\end{aligned}
$$

using $1-x\leq e^{-x}$. The final probabilities are summable, so Borel--Cantelli implies that eventually

$$
M_n>(1-\varepsilon)\log n.
$$

Intersecting over positive rational $\varepsilon$ proves the second [extremes of independent exponential variables](../../../../../../../extremes-of-independent-exponential-variables.md) assertion

$$
\boxed{\liminf_{n\to\infty}\frac{M_n}{\log n}\geq1}
\quad\hbox{almost surely}.
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [27G](../../../27g.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
