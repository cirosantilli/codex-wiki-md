# Edge contraction

↑ **Parent:** [Graph minor](graph-minor.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Edge_contraction)

An [edge contraction](edge-contraction.md) merges the two endpoints of an existing [edge](edge-of-a-graph.md). For a finite [simple graph](simple-graph.md) $G$ and $e=uv$, replace $u,v$ by a new [vertex](vertex-graph-theory.md) $w$. Retain every [edge](edge-of-a-graph.md) with neither endpoint in $\{u,v\}$, and join $w$ to every member of

$$
N_{G/e}(w)=(N_G(u)\cup N_G(v))\setminus\{u,v\}.
$$

Here $N_G(u)$ and $N_G(v)$ denote the original open [graph neighbourhoods](graph-neighbourhood.md), and $N_{G/e}(w)$ is the new [graph neighbourhood](graph-neighbourhood.md). Remove the [self-loop](loop-graph-theory.md) arising from $uv$ and merge duplicate [edges](edge-of-a-graph.md), so the result $G/e$ is again a [simple graph](simple-graph.md). This is not deletion of $uv$, which keeps both original [vertices](vertex-graph-theory.md).[The Basics (author-hosted chapter preview)](graph-theory-by-reinhard-diestel/the-basics-author-hosted-chapter-preview.md)

<a id="image-edge-contraction-of-a-four-cycle-and-a-triangle-in-a-graph-common-neighbours-determine-the-lost-edge-count"></a>
![](graph-edge-contraction-common-neighbour-count.png)

**[Figure 13](#image-edge-contraction-of-a-four-cycle-and-a-triangle-in-a-graph-common-neighbours-determine-the-lost-edge-count). Edge contraction of a four-cycle and a triangle in a graph: common neighbours determine the lost edge count**.

The left example contracts $uv$ in the [cycle graph](cycle-graph.md) $C_4$ to give $\{wa,ab,bw\}$. Its endpoints have no [common neighbours](common-neighbour.md), so four [edges](edge-of-a-graph.md) become three. The right example contracts $uv$ in the [triangle in a graph](triangle-in-a-graph.md) with [edges](edge-of-a-graph.md) $uv,ua,va$. Its endpoints have the single [common neighbour](common-neighbour.md) $a$, so the two [edges](edge-of-a-graph.md) $ua,va$ become one [edge](edge-of-a-graph.md) $wa$: three [edges](edge-of-a-graph.md) become one.

For any such [edge contraction](edge-contraction.md), the exact counts are

$$
|V(G/e)|=|V(G)|-1,\qquad |E(G/e)|=|E(G)|-1-|N_G(u)\cap N_G(v)|.
$$

The contracted [edge](edge-of-a-graph.md) accounts for one loss. Each [common neighbour](common-neighbour.md) $z$ contributes exactly one further loss, since $uz,vz$ become a single [edge](edge-of-a-graph.md) $wz$. All other [edges](edge-of-a-graph.md) correspond one-to-one to surviving [edges](edge-of-a-graph.md). In particular the new [degree of a vertex](degree-graph-theory.md) is

$$
\deg_{G/e}(w)=\deg_G(u)+\deg_G(v)-2-|N_G(u)\cap N_G(v)|.
$$

These formulas depend on simplifying to a [simple graph](simple-graph.md); a [multigraph](multigraph.md) convention that retains duplicate [edges](edge-of-a-graph.md) has different counts. In the six-[vertex](vertex-graph-theory.md) [branch set of a graph minor](branch-set-of-a-graph-minor.md) diagram, contracting $12$ loses one [edge](edge-of-a-graph.md), contracting the resulting $34$ loses two because of its [common neighbour](common-neighbour.md) $A$, and contracting $56$ loses one. Hence its seven [edges](edge-of-a-graph.md) become the three [edges](edge-of-a-graph.md) of $K_3$: $7-1-2-1=3$.

An [edge contraction](edge-contraction.md) can increase a [degree of a vertex](degree-graph-theory.md) even while decreasing both total counts. For example, contracting $uv$ in the [tree](tree-graph-theory.md) with [edges](edge-of-a-graph.md) $uv,ua,ub,vc,vd$ merges two [vertices](vertex-graph-theory.md) of [degree of a vertex](degree-graph-theory.md) three into one of [degree of a vertex](degree-graph-theory.md) four. This is the mechanism behind the distinction between a [graph minor](graph-minor.md) and a [topological minor](topological-minor.md).

## ↑ Ancestors (6)

1. [Graph minor](graph-minor.md)
2. [Graph theory](graph-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Branch set of a graph minor](branch-set-of-a-graph-minor.md)
- [Deletion-contraction recurrence for the chromatic polynomial](deletion-contraction-recurrence-for-the-chromatic-polynomial.md)
- [Edge contraction](edge-contraction.md)
- [Graph minor](graph-minor.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-110/4/solution.md)
- [Topological minor](topological-minor.md)
