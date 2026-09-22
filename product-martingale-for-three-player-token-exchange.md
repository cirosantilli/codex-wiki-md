# Product martingale for three-player token exchange

↑ **Parent:** [Martingale](martingale-split.md)

Three players with positive integer holdings exchange a token by choosing an unordered active pair uniformly, then choosing the transfer direction fairly. Let $N$ be the conserved total, and $\tau$ the [stopping time](stopping-time.md) of the first elimination. Given holdings $(x,y,z)$ before $\tau$, the [conditional expectation](conditional-expectation.md) of the change of their product is $-(x+y+z)/3=-N/3$: transfers in each pair decrease the mean product by the third holding. Thus the displayed [stopped process](stopped-process.md) is a [martingale](martingale-split.md). Its nonnegative product term gives $\mathbb E[n\wedge\tau]\leq3abc/N$, so the [monotone convergence theorem](monotone-convergence-theorem.md) first proves [integrability](integrability.md) of $\tau$. The bounded product then vanishes by the [dominated convergence theorem](dominated-convergence-theorem.md), yielding $\mathbb E[\tau]=3abc/N$. Continuing the deterministic time term beyond elimination instead produces a [submartingale](submartingale.md).

## ↑ Ancestors (6)

1. [Martingale](martingale-split.md)
2. [Probability theory](probability-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-probability-measure-and-martingales-course-of-the-university-of-oxford/2023/3/a/ii/solution.md)
