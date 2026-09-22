# Union by rank

↑ **Parent:** [Disjoint-set forest](disjoint-set-forest.md)

[Union by rank](union-by-rank.md) keeps a nonnegative [integer](integer-split.md) rank, initially zero, for each member. For each input, obtain its [root of a tree](root-of-a-tree.md) using the [disjoint-set find operation](disjoint-set-find-operation.md), then compare the resulting ranks. Attach the lower-rank [root of a tree](root-of-a-tree.md) below the higher-rank [root of a tree](root-of-a-tree.md), leaving both ranks unchanged. When the two [disjoint-set representatives](disjoint-set-representative.md) differ but their ranks are equal, choose either survivor and increase its rank by exactly one. A redundant [disjoint-set union operation](disjoint-set-union-operation.md) changes no ranks. [Path compression](path-compression.md) also changes no ranks. The surviving root's rank bounds the height of its [rooted tree](rooted-tree.md), measured in [edges](edge-of-a-graph.md); after [path compression](path-compression.md) it need not equal that height.[Robert Tarjan, COS 226 Bob’s Notes 1: Union-Find and Percolation, Version 2, Fall 2010, p. 4: rank linking, equal-rank increment and upper-bound interpretation after compression](cos-226-bob%E2%80%99s-notes-1-union-find-and-percolation-version-2-by-robert-tarjan.md)

In our example, let the first argument's [root of a tree](root-of-a-tree.md) survive equal-rank ties. The first two merges create roots $2,4$, each of rank $1$. The third gives $\mathrm{parent}[4]=2$ and increases the rank of $2$ to $2$. The fourth creates root $6$ of rank $1$. The fifth attaches $6$ below $2$ without increasing any rank. Before any subsequent compression queries, the indexed [arrays](array-data-structure.md) are

$$
\begin{array}{c|rrrrrrr}
x&1&2&3&4&5&6&7\\\hline
\mathrm{parent}[x]&2&2&4&2&6&2&7\\
\mathrm{rank}[x]&0&2&0&1&0&1&0
\end{array}
$$

The redundant call on $1,2$ leaves these [arrays](array-data-structure.md) unchanged. In particular, the [disjoint-set representative](disjoint-set-representative.md) of $1$ is $2$, although $1$ is the [minimum](minimum-of-a-subset-of-a-total-order.md) member of its [block of a set partition](block-of-a-set-partition.md).

Two short arguments explain the rank invariant. First, a root of rank $r$ has at least $2^r$ members in its [block of a set partition](block-of-a-set-partition.md): rank zero starts with one, and increasing rank combines two disjoint [blocks of a set partition](block-of-a-set-partition.md) with at least $2^r$ members each. Unequal-rank linking only adds members. Thus every rank is at most $\lfloor\log_2 n\rfloor$ for $n$ stored members, using the [floor function](floor-function.md) and [logarithm](logarithm.md). Second, height is initially zero; unequal-rank linking adds at most one to the lower height, while equal-rank linking raises the available bound by one. [Path compression](path-compression.md) only shortens routes. These arguments prove a height bound, not the stronger [amortized analysis](amortized-analysis.md) below.

## ↑ Ancestors (5)

1. [Disjoint-set forest](disjoint-set-forest.md)
2. [Disjoint-set data structure](disjoint-set-data-structure.md)
3. [Data structure](data-structure-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Path compression](path-compression.md)
- [Union by rank](union-by-rank.md)
- [Union-find operation bounds](union-find-operation-bounds.md)
