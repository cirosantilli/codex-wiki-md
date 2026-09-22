<h1 id="r/2/i/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a closed [Eulerian trail](../../../../../../eulerian-trail.md), every visit to a [vertex](../../../../../../vertex-graph-theory.md) pairs one entering [edge](../../../../../../edge-of-a-graph.md) with one departing [edge](../../../../../../edge-of-a-graph.md), including the initial/final [vertex](../../../../../../vertex-graph-theory.md). Thus every [degree](../../../../../../degree-graph-theory.md) is even.

Conversely, in a finite [connected graph](../../../../../../connected-graph.md) with all degrees even, start at a [vertex](../../../../../../vertex-graph-theory.md) and follow unused [edges](../../../../../../edge-of-a-graph.md) until no extension is possible. The walk cannot stop away from its starting point: at a different endpoint an odd number of its incident [edges](../../../../../../edge-of-a-graph.md) would have been used, leaving at least one unused [edge](../../../../../../edge-of-a-graph.md) because its total [degree](../../../../../../degree-graph-theory.md) is even. Thus it closes. If any [edge](../../../../../../edge-of-a-graph.md) remains unused, [connectedness](../../../../../../connected-space.md) gives a [vertex](../../../../../../vertex-graph-theory.md) of the current closed trail incident with an unused [edge](../../../../../../edge-of-a-graph.md). Repeat the construction from that [vertex](../../../../../../vertex-graph-theory.md) in the unused-[edge](../../../../../../edge-of-a-graph.md) subgraph and splice the resulting closed trail into the first one. Finitely many [edges](../../../../../../edge-of-a-graph.md) make the procedure terminate in a closed trail using every [edge](../../../../../../edge-of-a-graph.md) exactly once.

Hence **a [connected](../../../../../../connected-space.md) finite [graph](../../../../../../graph-split.md) has an Eulerian circuit exactly when all degrees are even**. If “trail” is allowed to be open, the printed equivalence needs correction: a [connected graph](../../../../../../connected-graph.md) has an [Eulerian trail](../../../../../../eulerian-trail.md) when it has zero or two odd-[degree](../../../../../../degree-graph-theory.md) [vertices](../../../../../../vertex-graph-theory.md). A single [edge](../../../../../../edge-of-a-graph.md) is an immediate counterexample to the unqualified printed statement.

## ↑ Ancestors (14)

1. [B](../b.md)
2. [I](../../i.md)
3. [2](../../../2.md)
4. [R](../../../../r.md)
5. [2008](../../../../../2008-split.md)
6. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../../split.md)
7. [Probability, statistics and options II course of the University of Oxford](../../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Mathematics and statistics course of the University of Oxford](../../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
