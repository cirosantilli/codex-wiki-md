<h1 id="17f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A graph is [eulerian graph](../../../../../../eulerian-graph.md) if it has a closed trail containing every edge exactly once. For a graph with at least three vertices, the [Euler circuit criterion](../../../../../../euler-circuit-criterion.md) says that it is Eulerian exactly when it is connected and every vertex has even degree.

Necessity is immediate: each visit of a closed trail to a vertex uses one entering and one leaving edge, so the incident edges occur in pairs; the trail also joins every vertex incident with an edge. Conversely, start at any vertex and extend an edge-simple trail until no unused incident edge remains. Even degrees force this maximal trail to end where it began. If edges remain, connectedness supplies a vertex of this circuit incident with an unused edge. Construct another closed trail from there and splice it into the first. Repeating consumes every edge and gives an Euler circuit.

The [line graph](../../../../../../line-graph.md) $L(G)$ has vertex set $E(G)$, with two vertices adjacent when the corresponding edges of $G$ share an endpoint. If $G$ is connected and $r$-regular, then $L(G)$ is connected, and the vertex corresponding to an edge $uv$ has degree

$$
(d(u)-1)+(d(v)-1)=2r-2.
$$

Every degree is even, so the Euler circuit criterion makes $L(G)$ Eulerian.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [17F](../../17f.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
