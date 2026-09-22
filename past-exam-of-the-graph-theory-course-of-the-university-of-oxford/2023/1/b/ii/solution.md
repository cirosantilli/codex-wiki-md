<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

By part (i), choose a [matching in a graph](../../../../../matching-graph-theory-split.md) $M_1$ meeting all [vertices](../../../../../vertex-graph-theory.md) of [vertex degree](../../../../../degree-graph-theory.md) $\Delta$ in $A$. Interchanging the two [vertex sets](../../../../../vertex-set.md) gives a [matching in a graph](../../../../../matching-graph-theory-split.md) $M_2$ meeting all such [vertices](../../../../../vertex-graph-theory.md) in $B$. Consider the spanning [subgraph](../../../../../subgraph.md) $H$ with [edges](../../../../../edge-of-a-graph.md) $M_1\cup M_2$.

Every [vertex](../../../../../vertex-graph-theory.md) has [vertex degree](../../../../../degree-graph-theory.md) at most two in $H$. An [edge](../../../../../edge-of-a-graph.md) belonging to both [matchings in a graph](../../../../../matching-graph-theory-split.md) forms a whole two-[vertex](../../../../../vertex-graph-theory.md) [connected component of a graph](../../../../../component-graph-theory.md), since neither endpoint can meet another [edge](../../../../../edge-of-a-graph.md) of either [matching in a graph](../../../../../matching-graph-theory-split.md). On every other nontrivial [connected component of a graph](../../../../../component-graph-theory.md), the [edges](../../../../../edge-of-a-graph.md) alternate between $M_1$ and $M_2$, so the [connected component of a graph](../../../../../component-graph-theory.md) is a [graph path](../../../../../path-in-a-graph.md) or an even [graph cycle](../../../../../cycle-in-a-graph.md). We select one of the two [matchings in a graph](../../../../../matching-graph-theory-split.md) separately on each [connected component of a graph](../../../../../component-graph-theory.md).

On a [graph cycle](../../../../../cycle-in-a-graph.md), either choice covers every [vertex](../../../../../vertex-graph-theory.md). On a [graph path](../../../../../path-in-a-graph.md) with an odd number of [edges](../../../../../edge-of-a-graph.md), the first and last [edges](../../../../../edge-of-a-graph.md) belong to the same [matching in a graph](../../../../../matching-graph-theory-split.md); choose it, and it covers every [vertex](../../../../../vertex-graph-theory.md) of the [graph path](../../../../../path-in-a-graph.md). For a common [edge](../../../../../edge-of-a-graph.md), choose that [edge](../../../../../edge-of-a-graph.md).

It remains to treat a [graph path](../../../../../path-in-a-graph.md) with a positive even number of [edges](../../../../../edge-of-a-graph.md). Its endpoints lie in the same side of the [bipartite graph](../../../../../bipartite-graph-split.md). Every internal [vertex](../../../../../vertex-graph-theory.md) meets both [matchings in a graph](../../../../../matching-graph-theory-split.md). If both endpoints lie in $A$, choose $M_1$: every endpoint of [vertex degree](../../../../../degree-graph-theory.md) $\Delta$ must already be met by $M_1$, by its defining property. If both endpoints lie in $B$, choose $M_2$ for the same reason. Thus the choice meets all [vertices](../../../../../vertex-graph-theory.md) of [vertex degree](../../../../../degree-graph-theory.md) $\Delta$ in that [connected component of a graph](../../../../../component-graph-theory.md).

Finally, an isolated [vertex](../../../../../vertex-graph-theory.md) of $H$ cannot have [vertex degree](../../../../../degree-graph-theory.md) $\Delta$ in $G$, since it would have been met by $M_1$ or $M_2$. The union of the selected [edges](../../../../../edge-of-a-graph.md) over the [connected components of a graph](../../../../../component-graph-theory.md) is a [matching in a graph](../../../../../matching-graph-theory-split.md), because different [connected components of a graph](../../../../../component-graph-theory.md) have disjoint [vertex sets](../../../../../vertex-set.md). It meets every [vertex](../../../../../vertex-graph-theory.md) of [vertex degree](../../../../../degree-graph-theory.md) $\Delta$ in $G$. The useful mechanism is the [union of two matchings](../../../../../union-of-two-matchings.md) and its alternating [connected components of a graph](../../../../../component-graph-theory.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the graph theory course of the University of Oxford](../../../../split.md)
6. [Graph theory course of the University of Oxford](../../../../../graph-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
