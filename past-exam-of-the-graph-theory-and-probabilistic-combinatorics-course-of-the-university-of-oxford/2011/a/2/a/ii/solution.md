<h1 id="a/2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $\Delta=\Delta(G)$, which is at least two because $x$ has the two specified [neighbours](../../../../../../neighbour-of-a-vertex.md). Give $y$ and $z$ the same colour, say colour one; this is proper because they are nonadjacent.

Apply part (i) to the [connected](../../../../../../connectivity-graph-theory.md) [graph](../../../../../../graph-split.md) $G\setminus\{y,z\}$, with $x$ last. Colour its [vertices](../../../../../../vertex-graph-theory.md) greedily in the resulting order using a palette of $\Delta$ colours. Every [vertex](../../../../../../vertex-graph-theory.md) before $x$ has a [neighbour](../../../../../../neighbour-of-a-vertex.md) later in this order, so at most $\deg(v)-1\leq\Delta-1$ of its [neighbours](../../../../../../neighbour-of-a-vertex.md) have already received colours. At least one palette colour is available.

When $x$ is reached, all its [neighbours](../../../../../../neighbour-of-a-vertex.md) are coloured, but the two [neighbours](../../../../../../neighbour-of-a-vertex.md) $y,z$ have the same colour. Thus there are at most $\deg(x)-1\leq\Delta-1$ distinct forbidden colours. Colour $x$ with a remaining one. This constructs a proper [colouring](../../../../../../colouring-of-a-set.md) with

$$
\boxed{\chi(G)\leq\Delta(G).}
$$

The common colour on the two initial [vertices](../../../../../../vertex-graph-theory.md) replaces the usual need for an uncoloured [neighbour](../../../../../../neighbour-of-a-vertex.md) at the last greedy step.

This is [greedy colouring with two precoloured neighbours](../../../../../../greedy-colouring-with-two-precoloured-neighbours.md).

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [A](../../../../a.md)
5. [2011](../../../../../2011-split.md)
6. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../split.md)
7. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
8. [Year 4 of the mathematics course of the University of Oxford](../../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
