# Trifurcation boundary-counting lemma

↑ **Parent:** [Trifurcation vertex in percolation](trifurcation-vertex-in-percolation.md)

For a finite [graph vertex](vertex-graph-theory.md) [set](set-split.md) $W$ in a [locally finite graph](locally-finite-graph.md), let $\partial^+W$ be its exterior [graph neighbours](neighbour-of-a-vertex.md). The number of [trifurcation vertices in percolation](trifurcation-vertex-in-percolation.md) lying in $W$ is at most $|\partial^+W|$.

For each cluster meeting $W$, contract its [connected components of a graph](component-graph-theory.md) outside $W$ to terminal [graph vertices](vertex-graph-theory.md), keeping only those adjacent to $W$. The resulting incidence [graph](graph-split.md) is finite and connected. Each trifurcation [graph vertex](vertex-graph-theory.md) in $W$ separates at least three groups of terminals, because every infinite branch must leave the [finite set](finite-set.md) $W$. Take a minimal subtree connecting all terminals. Each such trifurcation is unavoidable in that subtree and has [degree of a vertex](degree-graph-theory.md) at least three. All leaves are terminals. The [tree](tree-graph-theory.md) identity $\sum_v(\deg(v)-2)=-2$ bounds the number of these branching [graph vertices](vertex-graph-theory.md) by the number of leaves minus two, hence by the number of terminals. Different terminals, even across different clusters, can be assigned different exterior [graph neighbours](neighbour-of-a-vertex.md). Summing proves the bound. For square boxes in $\mathbb Z^2$, the boundary has order $n$ and the volume has order $n^2$.

**Table of contents**

- [Forest proof of trifurcation boundary counting](forest-proof-of-trifurcation-boundary-counting.md)

## ↑ Ancestors (10)

1. [Trifurcation vertex in percolation](trifurcation-vertex-in-percolation.md)
2. [Uniqueness of the infinite percolation cluster](uniqueness-of-the-infinite-percolation-cluster.md)
3. [Percolation cluster](percolation-cluster.md)
4. [Bond percolation](bond-percolation-split.md)
5. [Percolation theory](percolation-theory.md)
6. [Probability theory](probability-theory-split.md)
7. [Probability and statistics](probability-and-statistics-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Boundary counting proof of percolation uniqueness](boundary-counting-proof-of-percolation-uniqueness.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-37/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-30/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-214/2/b/solution.md)
