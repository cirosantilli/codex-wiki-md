<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $W(C)=\sum_{i\in C}w_i$. If the two disjoint winning [coalitions](../../../../../coalition-game-theory.md) exchange players, the aggregate weight is conserved:

$$
W(C_1')+W(C_2')=W(C_1)+W(C_2)\ge2q.
$$

If both resulting [coalitions](../../../../../coalition-game-theory.md) lost, each weight would be strictly below $q$, making their sum strictly below $2q$. This is impossible. Thus **every [weighted voting game](../../../../../weighted-voting-game.md) has [swap robustness for disjoint winning coalitions](../../../../../swap-robustness-for-disjoint-winning-coalitions.md)**, even when the weights or quota are negative.

**The converse is false.** The four-player prime-cardinality game from part (a) has [swap robustness for disjoint winning coalitions](../../../../../swap-robustness-for-disjoint-winning-coalitions.md): swapping one player each way preserves each [coalition](../../../../../coalition-game-theory.md)'s [cardinality](../../../../../cardinality.md), so in fact both winning [coalitions](../../../../../coalition-game-theory.md) remain winning. Part (a) proves it is not a [weighted voting game](../../../../../weighted-voting-game.md).

Even imposing monotonicity would not repair the converse under the printed disjointness restriction. As a stronger counterexample, use five players and declare a [coalition](../../../../../coalition-game-theory.md) winning exactly when it contains player $1$ and contains either both $2,3$ or both $4,5$. This is a [simple cooperative game](../../../../../simple-cooperative-game.md), and all its winning [coalitions](../../../../../coalition-game-theory.md) contain player $1$, so no two are disjoint; the stated swap condition holds vacuously.

Nevertheless $\{1,2,3\}$ and $\{1,4,5\}$ win, while $\{1,2,4\}$ and $\{1,3,5\}$ lose. Both pairs contain every player the same total number of times. A weighted representation would therefore give

$$
\begin{aligned}
2w_1+w_2+w_3+w_4+w_5&\ge2q
&&\text{from the winning pair},\\
2w_1+w_2+w_3+w_4+w_5&<2q
&&\text{from the losing pair},
\end{aligned}
$$

a contradiction. This is a [trade obstruction to weighted voting](../../../../../trade-obstruction-to-weighted-voting.md) and pinpoints how weak the disjoint-only swap requirement is.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Computational game theory](../../../computational-game-theory-split.md)
4. [2023](../../../split.md)
5. [Past exam of the MSc in advanced computer science course of the University of Oxford](../../../../split.md)
6. [MSc in advanced computer science course of the University of Oxford](../../../../../msc-in-advanced-computer-science-course-of-the-university-of-oxford.md)
7. [Master's course of the University of Oxford](../../../../../master-s-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
