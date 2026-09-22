<h1 id="7/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Choose a [maximum matching](../../../../../maximum-cardinality-matching.md) $M$ and a [minimum vertex cover](../../../../../minimum-vertex-cover.md) $C$. By [Kőnig's theorem for bipartite matching](../../../../../konig-s-theorem-graph-theory.md), $|M|=|C|$. Every [edge](../../../../../edge-of-a-graph.md) of $M$ must have at least one endpoint in $C$, because $C$ is a [vertex cover](../../../../../vertex-cover.md). Distinct [edges](../../../../../edge-of-a-graph.md) of the [matching in a graph](../../../../../matching-graph-theory-split.md) have disjoint endpoints, so these requirements already use at least $|M|$ distinct [vertices](../../../../../vertex-graph-theory.md) of $C$.

Since $C$ has exactly that many [vertices](../../../../../vertex-graph-theory.md), each [edge](../../../../../edge-of-a-graph.md) of $M$ has exactly one endpoint in $C$, and no [vertex](../../../../../vertex-graph-theory.md) of $C$ lies outside the endpoints of $M$. Thus selecting the unique endpoint in $C$ from each [edge](../../../../../edge-of-a-graph.md) of $M$ produces precisely the [vertex cover](../../../../../vertex-cover.md) $C$:

$$
\boxed{C=\{\text{one chosen endpoint of each edge of }M\}.}
$$

The argument also covers an edgeless [graph](../../../../../graph-split.md): take both sets empty.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the short options course of the University of Oxford](../../../../split.md)
6. [Short options course of the University of Oxford](../../../../../short-options-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
