# Graphic matroid

↑ **Parent:** [Matroid](matroid.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Graphic_matroid)

For a finite [undirected graph](undirected-graph.md), the [graphic matroid](graphic-matroid.md) has its [edges](edge-of-a-graph.md) as the [ground set](ground-set.md). A [subset](subset.md) is a [matroid independent set](independent-set-of-a-matroid.md) when its [edges](edge-of-a-graph.md) form a [forest](forest.md) on the original [vertices](vertex-graph-theory.md), including isolated [vertices](vertex-graph-theory.md). Its [matroid bases](basis-of-a-matroid.md) give a [spanning tree](spanning-tree.md) in each [connected component of a graph](component-graph-theory.md); for a [connected graph](connected-graph.md), each [matroid basis](basis-of-a-matroid.md) is a [spanning tree](spanning-tree.md).

For a [graph triangle](triangle-in-a-graph.md) on [vertices](vertex-graph-theory.md) $P,Q,R$, label the [edges](edge-of-a-graph.md) $a=PQ$, $b=QR$, and $c=PR$, with weights $8,5,6$. The [empty set](empty-set.md), all singletons, and all pairs are [forests](forest.md); the triple contains the [graph cycle](cycle-in-a-graph.md) $P,Q,R,P$. Thus its eight [subsets](subset.md) have exactly the independence pattern checked in the [weighted three-vector matroid](weighted-three-vector-matroid.md), and the same fifteen exchange comparisons pass. The [matroid greedy algorithm](matroid-greedy-algorithm.md) chooses $PQ$, chooses $PR$, and rejects $QR$, producing the heaviest [spanning tree](spanning-tree.md), of weight $14$.

<a id="image-a-weighted-graph-triangle-admits-greedy-selection-of-a-matroid-basis-a-hereditary-independence-system-without-exchange-traps-a-greedy-algorithm-at-weight-10-instead-of-12"></a>
![](matroid-triangle-and-hereditary-greedy-obstruction.png)

**[Figure 4](#image-a-weighted-graph-triangle-admits-greedy-selection-of-a-matroid-basis-a-hereditary-independence-system-without-exchange-traps-a-greedy-algorithm-at-weight-10-instead-of-12). A weighted graph triangle admits greedy selection of a matroid basis; a hereditary independence system without exchange traps a greedy algorithm at weight $10$ instead of $12$**.

**Exchange outline.** Deleting [edges](edge-of-a-graph.md) cannot create a [graph cycle](cycle-in-a-graph.md). If [forests](forest.md) $I,J$ have $|I|<|J|$, some [edge](edge-of-a-graph.md) of $J$ joins different [connected components of a graph](component-graph-theory.md) of $I$: otherwise, within each such component, $J$ would have at most its number of [vertices](vertex-graph-theory.md) minus one [edges](edge-of-a-graph.md), giving $|J|\leq|I|$. Adding that [edge](edge-of-a-graph.md) keeps a [forest](forest.md). This is the [matroid independence axioms](matroid-independence-axioms.md) expressed through connectivity.

## ↑ Ancestors (5)

1. [Matroid](matroid.md)
2. [Combinatorics](combinatorics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Graphic matroid](graphic-matroid.md)
- [Ground set](ground-set.md)
- [Independent set of a matroid](independent-set-of-a-matroid.md)
- [Matroid](matroid.md)
