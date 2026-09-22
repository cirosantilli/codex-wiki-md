<h1 id="29k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The stock tree has $S_0=5$, first-period values $6,4$, and terminal successors $7,5$ from $6$ and $5,3$ from $4$. When $r=1/6$, the risk-free growth factor is $R=7/6$. At the upper time-one node, investing $6$ in the risk-free asset produces $7$ at time two, while one share bought for $6$ produces only $7$ or $5$.

Use the following predictable [self-financing portfolio](../../../../../../self-financing-portfolio.md). Hold nothing initially. If $S_1=6$, short one share and invest the proceeds $6$ in the risk-free asset; if $S_1=4$, continue to hold nothing. Its terminal payoff is

$$
7-S_2=
\begin{cases}
0,&S_2=7,\\
2,&S_2=5
\end{cases}
$$

on the upper branch, and zero on the lower branch. It costs zero, is never negative, and is positive with positive probability, so it is an [arbitrage](../../../../../../arbitrage.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [29K](../../29k.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
