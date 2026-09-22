<h1 id="19h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A feasible flow assigns $f_{ij}$ to each directed edge so that

$$
0\leq f_{ij}\leq C_{ij}
$$

and inflow equals outflow at every vertex other than the source and sink. Its value $|f|$ is the net outflow from the source. For a set $S$ containing the source but not the sink, the associated cut has capacity

$$
C(S,V\setminus S)
=\sum_{i\in S,\,j\notin S}C_{ij}.
$$

The [max-flow min-cut theorem](../../../../../../max-flow-min-cut-theorem.md) states

$$
\boxed{
\max_f|f|=\min_{S\ni s,\,t\notin S}C(S,V\setminus S)}.
$$

For every flow and cut, conservation at vertices inside $S$ gives

$$
|f|=f(S,V\setminus S)-f(V\setminus S,S)
\leq C(S,V\setminus S).
$$

This proves the weak inequality.

A maximum flow exists because the feasible-flow polytope is nonempty, closed, and bounded. Form its residual graph: a forward edge has residual capacity $C_{ij}-f_{ij}$, and a reverse edge has residual capacity $f_{ij}$. If the residual graph contained a source-to-sink path, augmenting by the smallest positive residual capacity on that path would increase the flow, contradicting maximality.

Let $S$ be the vertices reachable from the source in the residual graph. The sink is not in $S$. Every original edge from $S$ to its complement is saturated, and every original edge from the complement into $S$ carries zero flow; otherwise the appropriate residual edge would make its other endpoint reachable. Hence

$$
|f|=f(S,V\setminus S)-f(V\setminus S,S)
=C(S,V\setminus S).
$$

The maximum flow therefore equals the capacity of this cut, completing the proof.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [19H](../../19h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
