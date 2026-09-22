<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

At each [vertex](../../../../../../vertex-graph-theory.md) independently, take a uniformly random permutation of the other $n-1$ [vertices](../../../../../../vertex-graph-theory.md). Use its first two entries for the two-out choices and its first $k$ entries for the $k$-out choices. Every unordered choice set has the prescribed [uniform distribution](../../../../../../continuous-uniform-distribution.md), and choices at different [vertices](../../../../../../vertex-graph-theory.md) remain [independent](../../../../../../independent-random-variables.md). This couples the [random k-out graphs](../../../../../../random-k-out-graph.md) so that $G_{2\text{-out}}\subseteq G_{k\text{-out}}$ on the same [vertex](../../../../../../vertex-graph-theory.md) set. Adding [edges](../../../../../../edge-of-a-graph.md) cannot destroy [graph](../../../../../../graph-split.md) connectivity. Consequently

$$
\boxed{\Pr(G_{k\text{-out}}\text{ connected})\ge\Pr(G_{2\text{-out}}\text{ connected})\longrightarrow1\quad(k\ge2).}
$$

This establishes [connectivity of random k-out graphs](../../../../../../connectivity-of-random-k-out-graphs.md) for every fixed allowed $k$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 12](../../../paper-12-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
