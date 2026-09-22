<h1 id="d6/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For the **[Watts-Strogatz model](../../../../../../watts-strogatz-model.md)**, choose $n$ [vertices](../../../../../../vertex-graph-theory.md) on a ring, an even initial [vertex degree](../../../../../../degree-graph-theory.md) $K<n$, and a rewiring [probability](../../../../../../probability.md) $p$. Connect each [vertex](../../../../../../vertex-graph-theory.md) to its $K/2$ nearest neighbours on each side. Consider each original clockwise [edge](../../../../../../edge-of-a-graph.md) once: with [probability](../../../../../../probability.md) $p$, retain its starting endpoint and replace its other endpoint uniformly, excluding [self-loops](../../../../../../loop-graph-theory.md) and duplicate [edges](../../../../../../edge-of-a-graph.md). The edge count remains $nK/2$, although individual [vertex degrees](../../../../../../degree-graph-theory.md) change.

Increasing $n$ at fixed $K$ lengthens unrewired-ring [graph distances](../../../../../../distance-graph-theory.md). Increasing $K$ adds [edges](../../../../../../edge-of-a-graph.md) and shortens distances. Increasing $p$ introduces shortcuts, sharply reducing [average shortest path length](../../../../../../average-shortest-path-length.md) at first, then progressively reducing the [clustering coefficient](../../../../../../clustering-coefficient.md) by destroying local triangles.

**The [small-world network](../../../../../../small-world-network.md) regime occurs at intermediate $p$** with sufficient shortcuts, substantial clustering, and $K\ll n$. At $p=0$ distances are long; near $p=1$ the clustering advantage disappears. The [degree distribution](../../../../../../degree-distribution.md) remains concentrated around $K$, so this is **not a [scale-free network](../../../../../../scale-free-network.md)**.[pp. 440–441, construction and dependence on rewiring probability](../../../../../../collective-dynamics-of-small-world-networks-by-duncan-j-watts-and-steven-h-strogatz.md)

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [D6](../../../d6.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../../split.md)
7. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
