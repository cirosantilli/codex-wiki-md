<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Continuity on the compact interval ensures that a maximum time exists. Fix a rational $r\in(0,1)$ and define

$$
U_r=\max_{0\leq t\leq r}B_t-B_r,
\qquad
V_r=\max_{r\leq t\leq1}(B_t-B_r).
$$

By Brownian time reversal and the [Brownian running maximum](../../../../../../brownian-running-maximum.md) law, $U_r\stackrel d=|N(0,r)|$. Independent increments give $V_r\stackrel d=|N(0,1-r)|$ independently of $U_r$. Their continuous distributions imply $\mathbb P(U_r=V_r)=0$.

If the maximum were attained at two distinct times, a rational $r$ strictly between them would make the maxima on $[0,r]$ and $[r,1]$ equal, hence $U_r=V_r$. A countable union over rational $r$ still has probability zero. Therefore the [time of the Brownian maximum](../../../../../../time-of-the-brownian-maximum.md) is almost surely unique.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
