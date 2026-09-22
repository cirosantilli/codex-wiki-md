<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

An [induced subgraph game](../../../../../induced-subgraph-game.md) is a [transferable utility game](../../../../../transferable-utility-game.md) represented by a weighted [undirected graph](../../../../../undirected-graph.md) with one [vertex](../../../../../vertex-graph-theory.md) per player; a [coalition](../../../../../coalition-game-theory.md)'s value is the sum of the [edge weights](../../../../../edge-weight.md) in its [induced subgraph](../../../../../induced-subgraph.md). With no [self-loops](../../../../../loop-graph-theory.md),

$$
\boxed{v(S)=\sum_{\{i,j\}\subseteq S,\ i\ne j}w_{ij},}
$$

where each unordered pair is counted once and an absent [edge](../../../../../edge-of-a-graph.md) has weight zero. Weights may have either sign. In an [induced subgraph game with self-loops](../../../../../induced-subgraph-game-with-self-loops.md), write the loop weight at $i$ as $\ell_i$ and add $\sum_{i\in S}\ell_i$, counting each loop once. In particular, $v(\{i\})=\ell_i$ when loops are allowed and is zero otherwise.[§1, printed p. 258: weighted induced-subgraph representation; the self-loop extension is stated explicitly here](../../../../../on-the-complexity-of-cooperative-solution-concepts-by-xiaotie-deng-and-christos-papadimitriou.md)

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Computational game theory](../../../computational-game-theory-split.md)
4. [2020](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
