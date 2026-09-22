<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $A_\Delta=\{a\in A:d_G(a)=\Delta\}$. Apply [Hall's marriage theorem](../../../../../hall-s-marriage-theorem.md) to the [induced subgraph](../../../../../induced-subgraph.md) on $A_\Delta\cup B$, which is a [bipartite graph](../../../../../bipartite-graph-split.md). For any [subset](../../../../../subset.md) $S\subseteq A_\Delta$, [double counting](../../../../../double-counting-proof-technique.md) the [edges](../../../../../edge-of-a-graph.md) from $S$ to its [graph neighbourhood](../../../../../graph-neighbourhood.md) gives

$$
\Delta|S|=\sum_{a\in S}d_G(a)=e_G(S,N(S))
\leq\sum_{b\in N(S)}d_G(b)\leq\Delta|N(S)|.
$$

The equality uses the fact that every [neighbour](../../../../../neighbour-of-a-vertex.md) of $S$ lies in $B$, so all [edges](../../../../../edge-of-a-graph.md) incident with $S$ have been counted. The final inequality uses the [maximum degree](../../../../../maximum-degree.md) bound on $B$. Since $\Delta>0$, division gives the [Hall condition](../../../../../hall-condition.md) $|S|\leq|N(S)|$.

Consequently there is a [matching in a graph](../../../../../matching-graph-theory-split.md) $M_1$ saturating $A_\Delta$. If $A_\Delta$ is empty, use the empty [matching in a graph](../../../../../matching-graph-theory-split.md). This proves the required [matching covering maximum-degree vertices in a bipartite graph](../../../../../matching-covering-maximum-degree-vertices-in-a-bipartite-graph.md) on the specified side; other [vertices](../../../../../vertex-graph-theory.md) need not be met.

## ↑ Ancestors (13)

1. [I](../i.md)
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
