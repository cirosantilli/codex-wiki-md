<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let the [bipartite graph](../../../../../../bipartite-graph.md) have parts $L,R$. Add a source $s$, a sink $t$, capacity-one edges $s\to u$ for $u\in L$ and $v\to t$ for $v\in R$, and capacity $M=|V|+1$ on each original edge directed $L\to R$. Use the [max-flow min-cut theorem](../../../../../../max-flow-min-cut-theorem.md): maximum flow value equals minimum cut capacity. Also use [Integrality of the Ford-Fulkerson algorithm](../../../../../../integrality-of-the-ford-fulkerson-algorithm.md): integral capacities admit an integral maximum flow, found by integral [augmenting paths](../../../../../../augmenting-path.md).

An integral flow selects a [matching in a graph](../../../../../../matching-graph-theory.md), because each left and right vertex carries at most one unit. Conversely every matching gives a unit flow along its selected $s\to u\to v\to t$ paths. Hence maximum flow value equals maximum matching cardinality.

A minimum cut has capacity at most $|L|$, whereas crossing even one original edge would cost $M>|L|$. For its source side $Z$, no edge of the original graph runs from $L\cap Z$ to $R\setminus Z$. Therefore

$$
U=(L\setminus Z)\cup(R\cap Z)
$$

is a [vertex cover](../../../../../../vertex-cover.md), and its cardinality is exactly the cut capacity. Conversely, given any cover $U$, use $Z=\{s\}\cup(L\setminus U)\cup(R\cap U)$. No original edge crosses this cut, because both its endpoints would otherwise be outside the cover; its capacity is $|U|$. Thus minimum cut capacity equals minimum cover size, proving [Kőnig's theorem for bipartite matching](../../../../../../konig-s-theorem-graph-theory.md):

$$
\boxed{\text{maximum matching size}=\text{minimum vertex-cover size}.}
$$

For the algorithm, repeatedly find [augmenting paths](../../../../../../augmenting-path.md) in the [residual network](../../../../../../residual-network.md), then take $Z$ to be the vertices reachable from $s$. Each integral augmentation increases flow by at least one; the total value is at most $\min(|L|,|R|)$. Each reachability search takes $O(|V|+|E|)$ time, so this procedure takes $O(|V|(|V|+|E|))$ time. The network uses only polynomially many edges and integer capacities, yielding the requested [polynomial-time algorithm](../../../../../../polynomial-time-algorithm.md) and an explicit cover.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
