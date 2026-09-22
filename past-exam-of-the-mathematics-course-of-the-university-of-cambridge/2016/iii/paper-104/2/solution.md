<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [topological graph](../../../../../graph-topology.md) is a [CW complex](../../../../../cw-complex.md) with only zero-dimensional and one-dimensional cells: its vertices form the zero-skeleton, and each edge is a copy of an open interval attached by its two endpoints to vertices, possibly the same vertex. It has the [weak topology of a CW complex](../../../../../weak-topology-of-a-cw-complex.md). A [subgraph](../../../../../subgraph.md) is a [CW subcomplex](../../../../../cw-subcomplex.md), obtained by choosing vertices and edges and retaining the endpoints of every chosen edge. Loops and multiple edges are allowed.

A [spanning tree](../../../../../spanning-tree.md) is a connected [spanning subgraph](../../../../../spanning-subgraph.md) containing no [cycle in a graph](../../../../../cycle-in-a-graph.md). To construct one in any connected [topological graph](../../../../../graph-topology.md) $\Gamma$, consider all acyclic spanning subgraphs, ordered by inclusion; the subgraph with every vertex and no edges is one. The union of a chain is still acyclic, since any cycle uses only finitely many edges and would already occur in a member of the chain. The [Zorn lemma](../../../../../zorn-s-lemma.md) therefore gives a maximal such subgraph $\Delta$.

If $\Delta$ were disconnected, a finite edge path in $\Gamma$ between vertices of two of its components would contain an edge joining different components. Adding that edge creates no cycle, contradicting maximality. Thus $\Delta$ is a [spanning tree](../../../../../spanning-tree.md). Fix a root vertex. Each point of $\Delta$ has a unique finite path to the root; give every edge length one and move the point a fraction $s$ of the way along that path at time $s\in[0,1]$. This defines a [contraction of a topological space](../../../../../contraction-of-a-topological-space.md) of $\Delta$. On each closed edge times $[0,1]$, the construction takes place in a finite tree and is continuous. Since the interval is a locally finite [CW complex](../../../../../cw-complex.md), the product with $\Delta$ has the corresponding [weak topology of a CW complex](../../../../../weak-topology-of-a-cw-complex.md), so these restrictions establish continuity globally. Consequently

$$
\boxed{\Delta\simeq\{\text{point}\}.}
$$

This argument includes infinite graphs and does not assume local finiteness of $\Gamma$.

If $p:\widetilde\Gamma\to\Gamma$ is a [covering map](../../../../../covering-space.md), take $p^{-1}(\Gamma^0)$ as the vertices upstairs. Each component of the inverse image of an open edge is an open interval mapping homeomorphically to that edge, because an interval is [simply connected](../../../../../simply-connected-space.md). Its parametrization lifts along the closed edge to attach its endpoints to lifted vertices, by [path lifting theorem](../../../../../path-lifting-theorem.md). Small star neighborhoods at vertices are lifted homeomorphically by the [covering map](../../../../../covering-space.md), and give exactly the neighborhoods of the resulting [topological graph](../../../../../graph-topology.md). Thus the cell structure has the topology of the original covering space. The total space may be disconnected, but every component is a [topological graph](../../../../../graph-topology.md).

The [Nielsen–Schreier formula](../../../../../nielsen-schreier-formula.md) is

$$
\boxed{[F_n:H]=d<\infty\quad\Longrightarrow\quad H\cong F_{1+d(n-1)}.}
$$

For a proof, realize $F_n$ as the [fundamental group](../../../../../fundamental-group.md) of the [wedge sum](../../../../../wedge-sum.md) of $n$ circles. Construct its connected [covering graph](../../../../../covering-graph.md) with vertices the right [cosets](../../../../../coset.md) $Hg$, and an oriented edge labeled $x_i$ from $Hg$ to $Hgx_i$ for each free generator $x_i$. There is exactly one incoming and one outgoing edge of each label at every vertex, which establishes the local [covering map](../../../../../covering-space.md) property. Reading a word from $H$ ends at its coset, so the closed paths at $H$ give exactly the words in $H$. The induced map of [fundamental groups](../../../../../fundamental-group.md) is injective by the [homotopy lifting property](../../../../../homotopy-lifting-property.md) of a [covering map](../../../../../covering-space.md), and its image is $H$.

For index $d$, this [covering graph](../../../../../covering-graph.md) has $d$ vertices and $dn$ edges. A [spanning tree](../../../../../spanning-tree.md) in it has $d-1$ edges. The permitted rank formula for a finite connected graph now gives

$$
\operatorname{rank}H=dn-(d-1)=1+d(n-1).
$$

In particular this proves both freeness and the index formula.

If $n\ge2$ and $d>1$, then $1+d(n-1)>n$, so a proper finite-index [subgroup](../../../../../subgroup.md) cannot be isomorphic to $F_n$. For $n=1$, $F_1\cong\mathbb Z$, and $d\mathbb Z$ is a proper index-$d$ [subgroup](../../../../../subgroup.md) isomorphic to $\mathbb Z$ for every $d\ge2$. Hence

$$
\boxed{\text{Such a proper finite-index copy exists exactly when }n=1.}
$$

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 104](../../paper-104-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
