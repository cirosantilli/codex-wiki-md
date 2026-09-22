<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use [vertex splitting](../../../../../../vertex-splitting.md) to encode node failures as well as link failures. Replace each vertex $v$ by $v_{\rm in},v_{\rm out}$ and an internal arc $v_{\rm in}\to v_{\rm out}$. Give that arc capacity one for an intermediary node, and capacity $B=|E|+|V|+1$ for the client and servers. Replace an undirected link $uv$ by arcs $u_{\rm out}\to v_{\rm in}$ and $v_{\rm out}\to u_{\rm in}$, each of capacity one. Connect server outputs to a common sink with capacity $B$ and take $c_{\rm out}$ as source.

A minimum cut avoids capacity-$B$ arcs because failure of all original links provides a cheaper separating set. We can normalize its source side so that $v_{\rm out}$ being on that side implies $v_{\rm in}$ is also there: moving $v_{\rm in}$ to that side cannot increase the cut capacity, since its sole outgoing arc leads to $v_{\rm out}$. In such a cut, at most one direction of any original link crosses. Every unit internal arc crossing corresponds to failing its intermediary node; every unit link arc corresponds to failing that link. Their failures disconnect all servers, so the cut capacity is the cost of a real failure set.

Conversely remove the internal arcs of failed nodes and both arcs of failed links. The reachable-side cut contains only arcs corresponding to those failures, with at most one crossing orientation per failed link; its capacity is at most their number. The [max-flow min-cut theorem](../../../../../../max-flow-min-cut-theorem.md) thus identifies the minimum mixed failure count $\lambda_{\rm mix}$ exactly. Hence

$$
\boxed{\text{the network is }m\text{-safe if and only if }\lambda_{\rm mix}>m.}
$$

The split graph has $O(|V|)$ vertices and $O(|E|+|V|+|S|)$ arcs, so the same [Edmonds–Karp algorithm](../../../../../../edmonds-karp-algorithm.md) gives a polynomial-time decision procedure.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
