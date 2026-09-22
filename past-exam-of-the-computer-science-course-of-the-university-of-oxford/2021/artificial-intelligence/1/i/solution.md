<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

**For $N\ge3$, depth and history-[tree](../../../../../tree-graph-theory-split.md) size can be infinite, while a sufficient finite state bound is $2\cdot5^N$.** The number of possible completed histories also becomes unbounded. With [variables](../../../../../variable-mathematics.md) $p,q,r$, first let $A$ assign $p$ and $B$ assign $q$. Both can then keep flipping their own [variable](../../../../../variable-mathematics.md), leaving $r$ unassigned. After four such flips the same assignment, ownership and player-to-move recur. Arbitrarily many repetitions can precede assignment of $r$, so there are infinitely many distinct finite complete histories as well as legal infinite plays.

A state must now record ownership: for each [variable](../../../../../variable-mathematics.md) the possibilities are unassigned, $A$-owned false, $A$-owned true, $B$-owned false, and $B$-owned true. Include the player to move, since flips break the old link between turn parity and the number assigned. This gives

$$
\boxed{|V|\le2\cdot5^N.}
$$

Many encoded positions are unreachable, so this is an upper bound. Each nonterminal state has at most $2N$ legal moves: two assignments per unassigned [variable](../../../../../variable-mathematics.md) and one flip per [variable](../../../../../variable-mathematics.md) owned by the acting player. Thus the finite [directed graph](../../../../../directed-graph.md) has at most $2N|V|$ [edges](../../../../../edge-of-a-graph.md) even though its unrolled [game tree](../../../../../game-tree.md) is infinite. The $2^N$ possible final [Boolean valuations](../../../../../boolean-valuation.md) are unchanged, but they no longer count distinct plays or complete ownership states. For $N=1,2$, no player gets a legal opportunity to flip before all [variables](../../../../../variable-mathematics.md) are assigned, so the original finite bounds still apply.

## ↑ Ancestors (11)

1. [I](../i.md)
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
