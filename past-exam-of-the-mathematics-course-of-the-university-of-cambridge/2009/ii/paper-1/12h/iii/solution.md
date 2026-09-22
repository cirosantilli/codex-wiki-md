<h1 id="12h/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

By [Gibbs inequality](../../../../../../gibbs-inequality.md),

$$
g(a)=\sum_jp_j\log\frac{p_j}{u_j}-D(p\Vert a)\leq\sum_jp_j\log\frac{p_j}{u_j},
$$

with equality exactly when **$\boxed{a_j=p_j}$**. Put $q_j=u_j/U$, a [probability distribution](../../../../../../probability-distribution.md). The optimal [log-optimal multiplicative betting](../../../../../../log-optimal-multiplicative-betting.md) rate is

$$
\boxed{g_* =D(p\Vert q)-\log U.}
$$

For $U<1$ this is strictly positive by [Gibbs inequality](../../../../../../gibbs-inequality.md); taking $0<\varepsilon<g_*$ in the preceding [strong law of large numbers](../../../../../../strong-law-of-large-numbers.md) bound proves growth with probability tending to one.

For $U>1$ the casino can set $u_j=Up_j$. Every optimal return multiplier is then exactly $1/U$, so the fortune decreases deterministically as $fU^{-m}$. More generally $g_*=-\log U<0$ for that choice. **An arbitrary choice with $U>1$ need not cause decline.** For example, take $p_1=p_2=1/2$, $u_1=0.01$, $u_2=1.99$. Then $U=2$ but $g_*=(1/2)\log[0.25/(0.01\cdot1.99)]>0$. For any fixed positive $p$, making one $u_j$ sufficiently small while preserving $U$ also makes the optimal rate positive.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [12H](../../12h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
