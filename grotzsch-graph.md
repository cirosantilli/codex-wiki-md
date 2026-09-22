<h1 id="grotzsch-graph">Grötzsch graph</h1>

↑ **Parent:** [Mycielskian](mycielskian.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Grötzsch_graph)

The [Grötzsch graph](grotzsch-graph.md) is the [Mycielskian](mycielskian.md) of the five-[vertex](vertex-graph-theory.md) [cycle graph](cycle-graph.md). Take original [edges](edge-of-a-graph.md) $v_iv_{i+1}$, with indices interpreted modulo five; add $u_iv_{i-1},u_iv_{i+1}$ and $wu_i$ for every $i$. There are eleven [vertices](vertex-graph-theory.md) and twenty [edges](edge-of-a-graph.md): five original, ten between originals and [Mycielski shadow vertices](mycielski-shadow-vertex.md), and five from the [Mycielski apex](mycielski-apex.md).

Give $v_1,\ldots,v_5$ colours $(1,2,1,2,3)$, give each $u_i$ the colour of $v_i$, and give $w$ colour 4. This is a [proper vertex colouring](proper-vertex-coloring.md). The [Mycielskian chromatic increase](mycielskian-chromatic-increase.md) proves that three colours are impossible, so the [chromatic number](chromatic-number.md) is exactly four. The [Mycielskian triangle preservation](mycielskian-triangle-preservation.md) proves that this is a [triangle-free graph](triangle-free-graph.md). In particular its [clique number](clique-number.md) is only two, even though its [chromatic number](chromatic-number.md) is four.

<a id="image-from-a-three-colour-cycle-graph-to-the-four-colour-grotzsch-graph"></a>
![](mycielski-five-cycle-grotzsch-four-colouring.png)

**[Figure 6](#image-from-a-three-colour-cycle-graph-to-the-four-colour-grotzsch-graph). From a three-colour cycle graph to the four-colour Grötzsch graph**. The outer pentagon on the right retains the original [vertices](vertex-graph-theory.md); the inner ring contains [Mycielski shadow vertices](mycielski-shadow-vertex.md) and has no ring [edges](edge-of-a-graph.md). The central [Mycielski apex](mycielski-apex.md) receives colour 4. Numbers identify colours independently of the fills, and labels identify the [vertices](vertex-graph-theory.md). Crossings without dots are not [vertices](vertex-graph-theory.md).

The [Mycielski apex](mycielski-apex.md) has an [independent set](independent-set-graph-theory.md) as its [graph neighbourhood](graph-neighbourhood.md), yet all three old colours are needed there in any three-colour [proper vertex colouring](proper-vertex-coloring.md) of the [subgraph](subgraph.md) obtained by deleting it. Thus a locally easy group of mutually nonadjacent neighbours can carry globally incompatible colour requirements. Absence of [triangles in a graph](triangle-in-a-graph.md) alone cannot bound the [chromatic number](chromatic-number.md).

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
