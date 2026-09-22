# Topological minor

↑ **Parent:** [Graph minor](graph-minor-split.md)

A [topological minor](topological-minor.md) records a network pattern whose [vertices](vertex-graph-theory.md) remain individual junctions but whose [edges](edge-of-a-graph.md) may become longer routes. For finite [simple graphs](simple-graph.md), $H\preccurlyeq_{\mathrm{top}}G$ means that $G$ contains a [subgraph](subgraph.md) that is a [graph subdivision](graph-subdivision.md) of $H$ up to [graph isomorphism](graph-isomorphism.md). Equivalently, choose distinct [branch vertices of a graph subdivision](branch-vertex-of-a-graph-subdivision.md) $b_v\in V(G)$ for $v\in V(H)$ and a [graph path](path-in-a-graph.md) $P_{uv}$ from $b_u$ to $b_v$ for every $uv\in E(H)$. These are [internally vertex-disjoint paths](internally-vertex-disjoint-paths.md), and no internal [vertex](vertex-graph-theory.md) of any $P_{uv}$ is a [branch vertex of a graph subdivision](branch-vertex-of-a-graph-subdivision.md). Only endpoints corresponding to a shared target [vertex](vertex-graph-theory.md) may be shared.[§1.7, printed p. 18: subdivisions; printed p. 21: topological-minor embeddings](graph-theory-by-reinhard-diestel/the-basics-author-hosted-chapter-preview.md)

The [graph subdivision](graph-subdivision.md) example below replaces two [edges](edge-of-a-graph.md) of a [triangle in a graph](triangle-in-a-graph.md) by routes of two and three [edges](edge-of-a-graph.md) while retaining its attached [leaf of a graph](leaf-of-a-graph.md). If the host [graph](graph-split.md) also contains an extra [edge](edge-of-a-graph.md) $BD$, the same routes still witness a [topological minor](topological-minor.md): delete $BD$ when selecting the [subgraph](subgraph.md). An [induced subgraph](induced-subgraph.md) is not required. However, routes that merely connect the right pairs are insufficient: using a [branch vertex of a graph subdivision](branch-vertex-of-a-graph-subdivision.md) as an intermediate junction, or making two routes share an internal [vertex](vertex-graph-theory.md), can change the local network structure.

Every [topological minor](topological-minor.md) is a [graph minor](graph-minor-split.md). In each [branch path of a graph subdivision](branch-path-of-a-graph-subdivision.md), contract all but one [edge](edge-of-a-graph.md); the disjoint interiors let this shorten each route without merging distinct [branch vertices of a graph subdivision](branch-vertex-of-a-graph-subdivision.md). This recovers $H$ after deleting unused [vertices](vertex-graph-theory.md) and [edges](edge-of-a-graph.md).[Proposition 1.7.3(i), printed p. 21](graph-theory-by-reinhard-diestel/the-basics-author-hosted-chapter-preview.md) The converse fails because an ordinary [branch set of a graph minor](branch-set-of-a-graph-minor.md) can gather several junctions into one.

For the [tree](tree-graph-theory-split.md) $T$ with [vertices](vertex-graph-theory.md) $u,v,a,b,c,d$ and [edges](edge-of-a-graph.md) $uv,ua,ub,vc,vd$, contracting $uv$ produces a [star graph](star-graph-theory.md) $K_{1,4}$: the [branch sets of a graph minor](branch-set-of-a-graph-minor.md) are $\{u,v\},\{a\},\{b\},\{c\},\{d\}$. Both $u,v$ have [degree of a vertex](degree-graph-theory.md) three; each of the other four [vertices](vertex-graph-theory.md) is a [leaf of a graph](leaf-of-a-graph.md) with [degree of a vertex](degree-graph-theory.md) one. The new centre $w$ has four distinct [graph neighbours](neighbour-of-a-vertex.md) $a,b,c,d$; its [degree of a vertex](degree-graph-theory.md) is $3+3-2=4$, in agreement with the [edge contraction](edge-contraction.md) formula.

<a id="image-a-graph-minor-can-combine-two-junctions-contracting-uv-creates-a-star-graph-with-a-centre-of-degree-of-a-vertex-four"></a>
![](topological-minor-tree-contraction-degree-obstruction.png)

**[Figure 1](#image-a-graph-minor-can-combine-two-junctions-contracting-uv-creates-a-star-graph-with-a-centre-of-degree-of-a-vertex-four). A graph minor can combine two junctions: contracting $uv$ creates a star graph with a centre of degree of a vertex four**.

Yet $K_{1,4}$ is not a [topological minor](topological-minor.md) of $T$. In a [graph subdivision](graph-subdivision.md) of $K_{1,4}$, four [branch paths of a graph subdivision](branch-path-of-a-graph-subdivision.md) must leave the centre through four different [edges](edge-of-a-graph.md); sharing their first internal [vertex](vertex-graph-theory.md) would violate internal disjointness. Thus any host needs a [vertex](vertex-graph-theory.md) of [degree of a vertex](degree-graph-theory.md) at least four, whereas $\Delta(T)=3$. More generally, $H\preccurlyeq_{\mathrm{top}}G$ implies $\Delta(H)\leq\Delta(G)$, where $\Delta$ is the [maximum degree of a graph](maximum-degree-of-a-graph.md). This bound concerns the host [graph](graph-split.md); extra unused [edges](edge-of-a-graph.md) may make its [branch vertices of a graph subdivision](branch-vertex-of-a-graph-subdivision.md) have larger [degrees of vertices](degree-graph-theory.md) than their target counterparts.

This distinction matters when a network's individual junctions have a limited number of connections: replacing a connection by a route preserves the number of routes meeting at each chosen junction, while contracting a connected region can combine connections from separate junctions. It also explains why a small nonplanar pattern can hide inside long routes. By [Kuratowski's theorem](kuratowski-s-theorem.md), a finite [simple graph](simple-graph.md) is a [planar graph](planar-graph-split.md) exactly when it has neither the [complete graph](complete-graph.md) $K_5$ nor the [complete bipartite graph](complete-bipartite-graph.md) $K_{3,3}$ as a [topological minor](topological-minor.md). The obstruction is a [graph subdivision](graph-subdivision.md) inside the network, regardless of the number of intermediate [vertices](vertex-graph-theory.md).

## ↑ Ancestors (6)

1. [Graph minor](graph-minor-split.md)
2. [Graph theory](graph-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Edge contraction](edge-contraction.md)
- [Graph minor](graph-minor-split.md)
- [Kuratowski's theorem](kuratowski-s-theorem.md)
- [Topological minor](topological-minor.md)
