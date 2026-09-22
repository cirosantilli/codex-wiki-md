<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use [degree-preserving edge rewiring](../../../../../degree-preserving-edge-rewiring.md), often called a double-edge swap. Select two [edges](../../../../../edge-of-a-graph.md) $(u,v)$ and $(x,y)$ with four distinct endpoints, then replace them by $(u,y)$ and $(x,v)$, choosing the reconnection symmetrically. Reject a proposal that would create a [self-loop](../../../../../loop-graph-theory.md) or an already present edge if the target is a [simple graph](../../../../../simple-graph.md). Each endpoint loses one edge and gains one, so every [degree of a vertex](../../../../../degree-graph-theory.md), as well as the numbers of [vertices](../../../../../vertex-graph-theory.md) and [edges](../../../../../edge-of-a-graph.md), is preserved exactly.

Repeat many such random proposals to generate reference networks. With symmetric proposals, retaining rejected steps as self-transitions, the uniform distribution on the reachable degree-preserving realizations is stationary. Adequate mixing must be checked; a few successful swaps do not establish an independent random sample. Degree preservation alone does not preserve connectedness, so impose and check that extra restriction if the [graph distance](../../../../../distance-graph-theory.md) comparison requires connected networks.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [6](../../6.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../split.md)
6. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
