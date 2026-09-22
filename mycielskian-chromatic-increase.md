# Mycielskian chromatic increase

↑ **Parent:** [Mycielskian](mycielskian.md)

For a nonempty finite [simple graph](simple-graph.md), the upper bound copies an optimal [proper vertex colouring](proper-vertex-coloring.md) to its [Mycielski shadow vertices](mycielski-shadow-vertex.md) and gives the [Mycielski apex](mycielski-apex.md) a fresh colour. For the lower bound, suppose $\mu(G)$ uses $k=\chi(G)$ colours, with $w$ coloured $k$. Shadows avoid $k$. Replace colour $k$ at each original $v_i$ by $u_i$'s colour. Changed originals form an [independent set](independent-set-graph-theory.md); unchanged neighbours differ because $u_iv_j$ is an [edge](edge-of-a-graph.md). This [proper vertex colouring](proper-vertex-coloring.md) of $G$ uses $k-1$ colours, contradicting its [chromatic number](chromatic-number.md).[§4.1, Proposition 1 and proof, manuscript pp. 6–7](mycielski-graphs-and-pr-proofs-by-emre-yolcu-and-others.md)

The nonempty condition means $V(G)\ne\varnothing$, not $E(G)\ne\varnothing$. An edgeless $n$-[vertex](vertex-graph-theory.md) [graph](graph-split.md) with $n\geq1$ has [chromatic number](chromatic-number.md) one; its [Mycielskian](mycielskian.md) is a [star graph](star-graph-theory.md) on $w,u_1,\ldots,u_n$ together with $n$ [isolated vertices](isolated-vertex.md), and needs two colours. If $G$ has no [vertices](vertex-graph-theory.md), $\mu(G)$ is a single [vertex](vertex-graph-theory.md), so the same formula also holds with the convention $\chi(G)=0$.

## ↑ Ancestors (8)

1. [Mycielskian](mycielskian.md)
2. [Chromatic number](chromatic-number.md)
3. [Graph coloring](graph-coloring-split.md)
4. [Graph theory](graph-theory-split.md)
5. [Foundations of mathematics](foundations-of-mathematics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Grötzsch graph](grotzsch-graph.md)
- [Triangle-free graphs with arbitrarily large chromatic number](triangle-free-graphs-with-arbitrarily-large-chromatic-number.md)
