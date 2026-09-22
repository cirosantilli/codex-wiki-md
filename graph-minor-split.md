# Graph minor

↑ **Parent:** [Graph theory](graph-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Graph_minor)

A [graph minor](graph-minor-split.md) compresses connected regions of a [graph](graph-split.md) into single [vertices](vertex-graph-theory.md) while retaining selected connections between them. For finite [simple graphs](simple-graph.md), $H\preccurlyeq G$ means that some sequence of deleting [vertices](vertex-graph-theory.md), deleting [edges](edge-of-a-graph.md), and performing [edge contractions](edge-contraction.md) produces $H$ up to [graph isomorphism](graph-isomorphism.md). Deleting a [vertex](vertex-graph-theory.md) also deletes all its incident [edges](edge-of-a-graph.md); deleting an [edge](edge-of-a-graph.md) leaves its endpoints. The [edge contraction](edge-contraction.md) convention here removes resulting [self-loops](loop-graph-theory.md) and duplicate [edges](edge-of-a-graph.md).[The Basics (author-hosted chapter preview)](graph-theory-by-reinhard-diestel/the-basics-author-hosted-chapter-preview.md)

For an exact small example, let $G$ be the [cycle graph](cycle-graph.md) $C_4$ with [vertices](vertex-graph-theory.md) $u,v,a,b$ and [edges](edge-of-a-graph.md) $uv,va,ab,bu$. Contract $uv$ to a new [vertex](vertex-graph-theory.md) $w$. The surviving [edges](edge-of-a-graph.md) are $wa,ab,bw$, giving the [complete graph](complete-graph.md) $K_3$. Thus $K_3\preccurlyeq C_4$, although $C_4$ has no [triangle in a graph](triangle-in-a-graph.md) as a [subgraph](subgraph.md). The [branch sets of a graph minor](branch-set-of-a-graph-minor.md) are $\{u,v\},\{a\},\{b\}$, with the original [edges](edge-of-a-graph.md) $va,ab,bu$ witnessing all three required adjacencies. The first panel of the [edge contraction](edge-contraction.md) diagram shows this operation.

A [subgraph](subgraph.md) uses existing [vertices](vertex-graph-theory.md) and [edges](edge-of-a-graph.md); a [topological minor](topological-minor.md) permits a [graph subdivision](graph-subdivision.md) of the target as a [subgraph](subgraph.md), so target [edges](edge-of-a-graph.md) become [graph paths](path-in-a-graph.md) with mutually disjoint interiors and no target [vertex](vertex-graph-theory.md) in an interior. An ordinary [graph minor](graph-minor-split.md) permits whole connected [branch sets of a graph minor](branch-set-of-a-graph-minor.md) in place of target [vertices](vertex-graph-theory.md). Every [topological minor](topological-minor.md) is a [graph minor](graph-minor-split.md), by contracting the replacement [graph paths](path-in-a-graph.md).[Proposition 1.7.3(i)](graph-theory-by-reinhard-diestel/the-basics-author-hosted-chapter-preview.md)

The converse fails. Take the [tree](tree-graph-theory-split.md) with [edges](edge-of-a-graph.md) $uv,ua,ub,vc,vd$. Contracting $uv$ gives the [star graph](star-graph-theory.md) $K_{1,4}$. Yet the original [tree](tree-graph-theory-split.md) has [maximum degree](maximum-degree.md) three, whereas every [graph subdivision](graph-subdivision.md) of $K_{1,4}$ retains a centre of [degree of a vertex](degree-graph-theory.md) four. Hence $K_{1,4}$ is a [graph minor](graph-minor-split.md) but not a [topological minor](topological-minor.md) of this [tree](tree-graph-theory-split.md). The difference is that a connected [branch set of a graph minor](branch-set-of-a-graph-minor.md) may gather connections incident to several original [vertices](vertex-graph-theory.md).

The counts of [vertices](vertex-graph-theory.md) and [edges](edge-of-a-graph.md) never increase under these operations. However, the $C_4$ example shows that being a [bipartite graph](bipartite-graph-split.md) is not preserved: its [graph minor](graph-minor-split.md) $K_3$ contains an [odd cycle](odd-cycle.md). Its [chromatic number](chromatic-number.md) also increases from two to three. A [connected graph](connected-graph.md) stays connected under an [edge contraction](edge-contraction.md), because the image of each [graph path](path-in-a-graph.md) still connects its endpoints, but deletion can disconnect it. Thus one must check the particular [graph property](graph-property.md) before treating it as preserved by taking [graph minors](graph-minor-split.md).

Being a [planar graph](planar-graph-split.md) is preserved: in a crossing-free drawing, shrink a contracted [edge](edge-of-a-graph.md) and bring its incident [edges](edge-of-a-graph.md) into the merged [vertex](vertex-graph-theory.md); deletion merely removes parts of the drawing. This makes a nonplanar [graph minor](graph-minor-split.md) a certificate that the original [graph](graph-split.md) is nonplanar. More strongly, for a finite [simple graph](simple-graph.md), being a [planar graph](planar-graph-split.md) is equivalent to having neither the [complete graph](complete-graph.md) $K_5$ nor the [complete bipartite graph](complete-bipartite-graph.md) $K_{3,3}$ as a [graph minor](graph-minor-split.md). Finding the corresponding [branch sets of a graph minor](branch-set-of-a-graph-minor.md) settles nonplanarity even when no literal $K_5$ or $K_{3,3}$ [subgraph](subgraph.md) is present. The converse is a substantial theorem, rather than a consequence of preservation alone.[Theorem 4.4.6, equivalence of planarity and exclusion of K5 and K3,3 minors](graph-theory-by-reinhard-diestel/planar-graphs-author-hosted-chapter-preview.md)

**Table of contents**

- [Topological minor](topological-minor.md)
- [Rooted branch-set reduction](rooted-branch-set-reduction.md)
- [Complete graph minor density threshold](complete-graph-minor-density-threshold.md)
  - [Dense minor with bounded order and high minimum degree](dense-minor-with-bounded-order-and-high-minimum-degree.md)
- [Branch set of a graph minor](branch-set-of-a-graph-minor.md)
  - [Random branch-set construction of a complete graph minor](random-branch-set-construction-of-a-complete-graph-minor.md)
- [Edge contraction](edge-contraction.md)

## ↑ Ancestors (5)

1. [Graph theory](graph-theory-split.md)
2. [Foundations of mathematics](foundations-of-mathematics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Dense minor with bounded order and high minimum degree](dense-minor-with-bounded-order-and-high-minimum-degree.md)
- [Edge contraction](edge-contraction.md)
- [Graph minor](graph-minor-split.md)
- [Kuratowski's theorem](kuratowski-s-theorem.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-9/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-110/4/solution.md)
- [Rooted dense minor linkage](rooted-dense-minor-linkage.md)
- [Topological minor](topological-minor.md)
- [Wheel graph](wheel-graph.md)
