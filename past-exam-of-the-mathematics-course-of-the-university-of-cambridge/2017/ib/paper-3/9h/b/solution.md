<h1 id="9h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the usual undirected graph with at least two vertices, a [simple random walk](../../../../../../simple-random-walk.md) chooses a neighbor uniformly at each step, so $P_{ij}=1/d_i$ when $i$ and $j$ are adjacent and zero otherwise, where $d_i$ is the [degree of a vertex](../../../../../../degree-graph-theory.md). The [handshaking lemma](../../../../../../degree-sum-formula.md) gives $\sum_id_i=2|E|$. Thus the [stationary distribution of a graph random walk](../../../../../../stationary-distribution-of-a-graph-random-walk.md) is

$$
\boxed{\pi_i=\frac{d_i}{2|E|}.}
$$

For adjacent $i,j$, $\pi_iP_{ij}=1/(2|E|)=\pi_jP_{ji}$, and for nonadjacent pairs both sides vanish. By [detailed balance](../../../../../../detailed-balance.md), this is an [invariant distribution](../../../../../../stationary-distribution.md) and the walk started from it is a [reversible Markov chain](../../../../../../reversible-markov-chain.md). Connectedness makes the finite walk an [irreducible Markov chain](../../../../../../irreducible-markov-chain.md), giving uniqueness of its [invariant distribution](../../../../../../stationary-distribution.md). No aperiodicity assumption is needed for uniqueness, so a bipartite graph is allowed.

If the connected graph has a single isolated vertex, the usual neighbor-choice formula is undefined. With the natural absorbing convention $P_{11}=1$, its unique [invariant distribution](../../../../../../stationary-distribution.md) is $\pi_1=1$ and it is reversible. The degree-normalization formula presupposes at least one edge.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [9H](../../9h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
