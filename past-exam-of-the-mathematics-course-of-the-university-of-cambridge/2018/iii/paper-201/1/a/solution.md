<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a discrete-time [martingale](../../../../../../martingale-split.md) $(M_n)$ and real $a<b$, let $U_N[a,b]$ be the [upcrossing count](../../../../../../upcrossing-count.md): buy on the first observation at or below $a$, sell on the next observation at or above $b$, and repeat up to time $N$, counting only completed pairs. Writing $z^-=max(-z,0)$, the [Doob upcrossing inequality](../../../../../../doob-upcrossing-inequality.md) is

$$
\boxed{(b-a)\mathbb E U_N[a,b]\leq\mathbb E(M_N-a)^-.}
$$

This convention permits the first purchase at time zero. Equivalently, the right side is $\mathbb E(M_N-a)^+-\mathbb E(M_0-a)$, because the [martingale](../../../../../../martingale-split.md) has constant [expected value](../../../../../../expected-value.md).

For completeness, let $H_k\in\{0,1\}$ indicate whether the trading rule holds one unit during $(k-1,k]$. This is a [predictable process](../../../../../../predictable-process.md), so the [martingale transform](../../../../../../martingale-transform.md) $G_N=\sum_{k=1}^NH_k(M_k-M_{k-1})$ has zero [expected value](../../../../../../expected-value.md). Every completed trade gains at least $b-a$, and an unfinished trade loses at most $(M_N-a)^-$. Thus $G_N\geq(b-a)U_N[a,b]-(M_N-a)^-$, giving the inequality.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
