<h1 id="3/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Start with all of $N_0$ and $N_1$, namely $-1,-1/2,-1/2$, whose sum is $-2$. For $n=0,1,2,\ldots$ in order, append $2^{n+1}$ copies of the triple

$$
\left(2^{-(n+1)},\ -2^{-(n+2)},\ -2^{-(n+2)}\right).
$$

This uses all $2^{n+1}$ occurrences of $P_n$ and all $2^{n+2}$ occurrences of $N_{n+2}$, exactly once. Together with the initial terms, every original occurrence is used, establishing a [rearrangement of a series](../../../../../../../rearrangement-of-a-series.md). Its beginning is

$$
-1,-\frac12,-\frac12,\quad
\frac12,-\frac14,-\frac14,\frac12,-\frac14,-\frac14,\quad\ldots.
$$

Each triple has sum zero. At its intermediate terms the [partial sum](../../../../../../../partial-sum.md) is at most $2^{-(n+1)}$ above $-2$. This bound tends to zero, so the whole [series](../../../../../../../series-mathematics.md), rather than just the [subsequence](../../../../../../../subsequence.md) of sums at completed triples, has sum $\boxed{-2}$.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [Mathematics II](../../../../mathematics-ii-split.md)
5. [Prelims](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
