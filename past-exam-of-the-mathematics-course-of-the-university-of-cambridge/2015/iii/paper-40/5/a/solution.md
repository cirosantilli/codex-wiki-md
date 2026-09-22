<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use a [telescoping replication of a stock-price sum](../../../../../../telescoping-replication-of-a-stock-price-sum.md). Hold $T-t+1$ shares during interval $(t-1,t]$; at time $t$, sell one share and keep its proceeds in the bond. Start with $T$ shares and no cash, costing $TS_0$.

After the time-$t$ rebalance, the [stock](../../../../../../stock.md) holdings are $T-t$ and the cash holdings are $\sum_{u=1}^tS_u$, so wealth is

$$
V_t=\sum_{u=1}^tS_u+(T-t)S_t.
$$

The sale of one share exactly funds the cash increase, making the strategy [self-financing](../../../../../../self-financing-portfolio.md). Equivalently,

$$
\boxed{TS_0+\sum_{t=1}^T(T-t+1)(S_t-S_{t-1})
=\sum_{u=1}^TS_u.}
$$

At time $T$ there are no remaining shares, and the cash equals the claim. All [stock](../../../../../../stock.md) positions over trading intervals are predictable.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
