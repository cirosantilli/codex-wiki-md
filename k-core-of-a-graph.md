# k-core of a graph

↑ **Parent:** [Graph theory](graph-theory-split.md)

For a nonnegative [integer](integer-split.md) $k$, the [k-core of a graph](k-core-of-a-graph.md) is the unique maximum by [set inclusion](set-inclusion.md) [induced subgraph](induced-subgraph.md) in which every [degree of a vertex](degree-graph-theory.md) is at least $k$, allowing the empty [graph](graph-split.md). Repeatedly delete [vertices](vertex-graph-theory.md) whose current [degree of a vertex](degree-graph-theory.md) is less than $k$. These [induced subgraphs](induced-subgraph.md) are nested: $C_{k+1}(G)\subseteq C_k(G)$; the case $k=2$ is the [2-core](2-core-of-a-graph.md). In their 2003 preprint, [Vladimir Batagelj](vladimir-batagelj.md) and [Matjaž Zaveršnik](matjaz-zaversnik.md) give an [algorithm](algorithm-split.md) for the entire core decomposition, using degree buckets and constant-time position updates. Their general bound is $O(|V|+|E|)$; the title's $O(m)$ form applies to [connected graphs](connected-graph.md) with at least two [vertices](vertex-graph-theory.md), where $m=|E|\geq|V|-1$. [Batagelj and Zaveršnik, An O(m) Algorithm for Cores Decomposition of Networks, §§2–4.1, especially Algorithm 1 and the general O(max(m,n)) bound](an-o-m-algorithm-for-cores-decomposition-of-networks-by-vladimir-batagelj-and-matjaz-zaversnik.md)

## ↑ Ancestors (5)

1. [Graph theory](graph-theory-split.md)
2. [Foundations of mathematics](foundations-of-mathematics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [K-core of a graph](k-core-of-a-graph.md)
- [Leaf pruning for the 2-core](leaf-pruning-for-the-2-core.md)
