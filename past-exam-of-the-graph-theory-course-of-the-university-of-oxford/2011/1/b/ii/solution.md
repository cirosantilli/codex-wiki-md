<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let the [bipartition](../../../../../bipartition-of-a-graph.md) be $L\cup R$. Form an auxiliary [graph](../../../../../graph-split.md) by adding a new [vertex](../../../../../vertex-graph-theory.md) $s$ adjacent to every [vertex](../../../../../vertex-graph-theory.md) of $L$ and a new [vertex](../../../../../vertex-graph-theory.md) $t$ adjacent to every [vertex](../../../../../vertex-graph-theory.md) of $R$. The [vertices](../../../../../vertex-graph-theory.md) $s,t$ are nonadjacent, so [Menger's theorem](../../../../../menger-theorem.md) applies.

A [matching](../../../../../matching-graph-theory-split.md) of size $m$ gives $m$ internally disjoint [graph paths](../../../../../path-in-a-graph.md) $s\ell rt$, one for each [matching](../../../../../matching-graph-theory-split.md) [edge](../../../../../edge-of-a-graph.md) $\ell r$. Conversely, every $s$-$t$ [graph path](../../../../../path-in-a-graph.md) must use an [edge](../../../../../edge-of-a-graph.md) of the original [bipartite graph](../../../../../bipartite-graph-split.md). Choose one such [edge](../../../../../edge-of-a-graph.md) from each member of an internally disjoint family. Their endpoints are all distinct, so the chosen [edges](../../../../../edge-of-a-graph.md) form a [matching](../../../../../matching-graph-theory-split.md). Thus the [maximum](../../../../../maximum-of-a-subset-of-a-total-order.md) number of those [graph paths](../../../../../path-in-a-graph.md) is the [maximum matching](../../../../../maximum-cardinality-matching.md) size.

An $s$-$t$ separator contained in $L\cup R$ is exactly a [vertex cover](../../../../../vertex-cover.md) of the original [graph](../../../../../graph-split.md). Indeed, an uncovered [edge](../../../../../edge-of-a-graph.md) $\ell r$ would leave the [graph path](../../../../../path-in-a-graph.md) $s\ell rt$, while removing a [vertex cover](../../../../../vertex-cover.md) removes every [edge](../../../../../edge-of-a-graph.md) between $L$ and $R$ and hence every $s$-$t$ [graph path](../../../../../path-in-a-graph.md). The [minimum](../../../../../minimum-of-a-subset-of-a-total-order.md) separator size is therefore the [minimum](../../../../../minimum-of-a-subset-of-a-total-order.md) [vertex cover](../../../../../vertex-cover.md) size. Menger gives

$$
\boxed{\nu(G)=\tau(G)\quad\text{for bipartite }G.}
$$

This is [Kőnig's theorem for bipartite matching](../../../../../konig-s-theorem-graph-theory.md). The auxiliary construction gives the required deduction from [vertex-disjoint paths](../../../../../vertex-disjoint-paths.md) rather than assuming a [matching](../../../../../matching-graph-theory-split.md) theorem in advance.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the graph theory course of the University of Oxford](../../../../split.md)
6. [Graph theory course of the University of Oxford](../../../../../graph-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
