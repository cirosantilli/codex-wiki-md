# Trade obstruction to weighted voting

↑ **Parent:** [Weighted voting game](weighted-voting-game.md)

Suppose winning [coalitions](coalition-game-theory.md) $W_1,\ldots,W_k$ and losing [coalitions](coalition-game-theory.md) $L_1,\ldots,L_k$ contain each player the same total number of times:

$$
\sum_{j=1}^{k}\mathbf1_{\{i\in W_j\}}
=\sum_{j=1}^{k}\mathbf1_{\{i\in L_j\}}
\quad\text{for every player }i.
$$

No real-weight, weak-quota [weighted voting game](weighted-voting-game.md) represents those outcomes. Summing weights over the winning family gives at least $kq$, while summing over the losing family gives strictly less than $kq$. Equal player multiplicities make the two sums identical, a contradiction. This certificate works without assuming nonnegative weights.

For example, the winners $\{1,2,3\},\{1,4,5\}$ and losers $\{1,2,4\},\{1,3,5\}$ form a two-against-two obstruction. A monotone game whose minimal winning [coalitions](coalition-game-theory.md) are the first two sets realizes this certificate, even though every winner contains player $1$.

## ↑ Ancestors (8)

1. [Weighted voting game](weighted-voting-game.md)
2. [Transferable utility game](transferable-utility-game.md)
3. [Cooperative game theory](cooperative-game-theory.md)
4. [Game theory](game-theory-split.md)
5. [Mathematical optimization](mathematical-optimization-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-msc-in-advanced-computer-science-course-of-the-university-of-oxford/2023/computational-game-theory/4/b/solution.md)
