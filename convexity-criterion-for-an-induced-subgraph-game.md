# Convexity criterion for an induced subgraph game

↑ **Parent:** [Induced subgraph game](induced-subgraph-game.md)

A loop-free [induced subgraph game](induced-subgraph-game.md) is a [convex cooperative game](convex-cooperative-game.md) exactly when all [edge weights](edge-weight.md) are nonnegative. Necessity follows by testing the [supermodular](supermodular-set-function.md) inequality on two distinct singleton [coalitions](coalition-game-theory.md). For sufficiency,

$$
v(S\cup T)+v(S\cap T)-v(S)-v(T)
=\sum_{i\in S\setminus T,\ j\in T\setminus S}w_{ij}\ge0.
$$

Only [edges](edge-of-a-graph.md) connecting the two set differences survive cancellation. Loop contributions cancel as well, so the same off-diagonal condition remains sufficient and necessary when [self-loops](loop-graph-theory.md) are added.

## ↑ Ancestors (8)

1. [Induced subgraph game](induced-subgraph-game.md)
2. [Transferable utility game](transferable-utility-game.md)
3. [Cooperative game theory](cooperative-game-theory.md)
4. [Game theory](game-theory-split.md)
5. [Mathematical optimization](mathematical-optimization-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2020/computational-game-theory/3/f/solution.md)
