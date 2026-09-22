# Mycielskian

↑ **Parent:** [Chromatic number](chromatic-number.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mycielskian)

The Mycielski construction replaces a graph $G$ with a graph $\mu(G)$ having one shadow vertex for each original vertex and one further vertex adjacent to every shadow. It satisfies

$$
\chi(\mu(G))=\chi(G)+1
$$

and preserves triangle-freeness. Iterating it from the five-cycle gives triangle-free graphs of arbitrarily large chromatic number.

Here $G$ is a finite [simple graph](simple-graph.md) with at least one [vertex](vertex-graph-theory.md); it need not have an [edge](edge-of-a-graph.md). The [Mycielskian](mycielskian.md) separates two ways of needing many colours: a large [clique](clique-graph-theory.md) forces distinct colours immediately, but a [triangle-free graph](triangle-free-graph.md) can impose incompatible choices through its whole pattern of [graph adjacency](graph-adjacency.md). The [Mycielski construction](mycielskian.md) increases that global constraint while preserving the absence of [triangles in a graph](triangle-in-a-graph.md).

Write the [vertex set](vertex-set.md) of $G$ as $\{v_1,\ldots,v_n\}$, with $n\geq1$. Keep these [vertices](vertex-graph-theory.md), add distinct [Mycielski shadow vertices](mycielski-shadow-vertex.md) $u_1,\ldots,u_n$, and add a [Mycielski apex](mycielski-apex.md) $w$. The [vertex set](vertex-set.md) and complete list of [edges](edge-of-a-graph.md) are

$$
\begin{aligned}
V(\mu(G))&=\{v_1,\ldots,v_n,u_1,\ldots,u_n,w\},\\
E(\mu(G))&=E(G)\cup\{\{u_i,v_j\},\{u_j,v_i\}:\{v_i,v_j\}\in E(G)\}\cup\{\{w,u_i\}:1\leq i\leq n\}.
\end{aligned}
$$

There are no other [edges](edge-of-a-graph.md): the [Mycielski shadow vertices](mycielski-shadow-vertex.md) form an [independent set](independent-set-graph-theory.md), $w$ has no original [vertex](vertex-graph-theory.md) as a neighbour, and $u_i$ is not adjacent to $v_i$. Each [Mycielski shadow vertex](mycielski-shadow-vertex.md) copies its original [vertex](vertex-graph-theory.md)'s [graph neighbourhood](graph-neighbourhood.md) within the original [vertex set](vertex-set.md), not its position in the drawing. This is the construction in the inspected research paper.[§4.1, manuscript pp. 5–6, construction steps 1–3](mycielski-graphs-and-pr-proofs-by-emre-yolcu-and-others.md)

For $n$ original [vertices](vertex-graph-theory.md) and $m$ original [edges](edge-of-a-graph.md), direct counting gives $2n+1$ [vertices](vertex-graph-theory.md) and $3m+n$ [edges](edge-of-a-graph.md). The original [vertices](vertex-graph-theory.md) induce a copy of $G$, so no original [graph adjacency](graph-adjacency.md) is lost. A drawing crossing is not an extra [vertex](vertex-graph-theory.md).

Start with the [complete graph](complete-graph.md) $K_2$, whose only [edge](edge-of-a-graph.md) is $v_1v_2$, abbreviating $\{v_1,v_2\}$. Its [Mycielskian](mycielskian.md) has exactly the [edges](edge-of-a-graph.md) $v_1v_2,u_1v_2,u_2v_1,wu_1,wu_2$. Reading them as $v_1,v_2,u_1,w,u_2,v_1$ gives the [cycle graph](cycle-graph.md) $C_5$. A [proper vertex colouring](proper-vertex-coloring.md) gives $v_1,u_1$ colour 1, $v_2,u_2$ colour 2, and $w$ colour 3. Two colours cannot close an [odd cycle](odd-cycle.md), so its [chromatic number](chromatic-number.md) is exactly three.

<a id="image-the-mycielski-construction-turns-the-complete-graph-k-2-into-the-cycle-graph-c-5"></a>
![](mycielski-single-edge-five-cycle-colouring.png)

**[Figure 5](#image-the-mycielski-construction-turns-the-complete-graph-k-2-into-the-cycle-graph-c-5). The Mycielski construction turns the complete graph $K_2$ into the cycle graph $C_5$**. Numbers inside the [vertices](vertex-graph-theory.md) are colours. Solid, dashed and dotted [edges](edge-of-a-graph.md) distinguish the original connection, copied neighbour constraints and [Mycielski apex](mycielski-apex.md) connections. The second drawing is a single [odd cycle](odd-cycle.md), with no [triangles in a graph](triangle-in-a-graph.md).

**Table of contents**

- [Grötzsch graph](grotzsch-graph.md)
- [Mycielski shadow vertex](mycielski-shadow-vertex.md)
- [Mycielski apex](mycielski-apex.md)
- [Mycielskian chromatic increase](mycielskian-chromatic-increase.md)
- [Mycielskian triangle preservation](mycielskian-triangle-preservation.md)
- [Triangle-free graphs with arbitrarily large chromatic number](triangle-free-graphs-with-arbitrarily-large-chromatic-number.md)

## ↑ Ancestors (7)

1. [Chromatic number](chromatic-number.md)
2. [Graph coloring](graph-coloring-split.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Grötzsch graph](grotzsch-graph.md)
- [Mycielskian](mycielskian.md)
- [Mycielskian chromatic increase](mycielskian-chromatic-increase.md)
- [Mycielskian triangle preservation](mycielskian-triangle-preservation.md)
