<h1 id="1/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

**Depth $N$; at most $2^N N!$ complete plays; $3^N$ partial-assignment states; and $\sum_{k=0}^N2^kN!/(N-k)!$ [tree](../../../../../tree-graph-theory-split.md) nodes.** Here “different games” means complete move histories for the fixed [propositional formula](../../../../../propositional-formula.md), rather than different syntactic formulas or merely different terminal [Boolean valuations](../../../../../boolean-valuation.md).

At depth $k$, the players have chosen an ordered list of $k$ distinct [variables](../../../../../variable-mathematics.md) and a truth value for each, giving

$$
L_k=\frac{N!}{(N-k)!}\,2^k.
$$

Thus complete histories number $L_N=2^N N!$: $N!$ [variable](../../../../../variable-mathematics.md) orders and $2^N$ assignments. Different [variable](../../../../../variable-mathematics.md) orders can reach the same terminal [Boolean valuation](../../../../../boolean-valuation.md), of which there are only $2^N$.

For a game state, each [variable](../../../../../variable-mathematics.md) is unassigned, false or true, giving $3^N$ possibilities. Ownership and variable-assignment order are irrelevant in this version, and the next player is determined by the parity of the number already assigned. The full [game tree](../../../../../game-tree.md), which keeps histories separate, has

$$
\boxed{\sum_{k=0}^N L_k=2^N N!\sum_{j=0}^N\frac1{2^j j!}<2^{N+1}N!.}
$$

The depth counts [edges](../../../../../edge-of-a-graph.md); there are $N+1$ levels. These bounds explore the full [tree](../../../../../tree-graph-theory-split.md) even when a formula's truth might be inferable from a partial assignment, since the stated stopping rule waits for all [variables](../../../../../variable-mathematics.md).

## ↑ Ancestors (11)

1. [G](../g.md)
2. [1](../../1.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2021](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
