# Trail in a graph

↑ **Parent:** [Walk in a graph](walk-in-a-graph.md)

A [trail](trail-in-a-graph.md) is a [walk](walk-in-a-graph.md) whose [edge](edge-of-a-graph.md) [sequence](sequence.md) $e_1,\ldots,e_m$ has no repetitions. Its [vertices](vertex-graph-theory.md) may repeat, including its first and last [vertices](vertex-graph-theory.md). The zero-length [walk](walk-in-a-graph.md) is a [trail](trail-in-a-graph.md) because it repeats no [edge](edge-of-a-graph.md). Every [graph path](path-in-a-graph.md) is a [trail](trail-in-a-graph.md), but the converse fails: the [trail](trail-in-a-graph.md) in the shared example is

$$
B,BC,C,CA,A,AD,D,DE,E,EA,A,AF,F.
$$

Its six [edges](edge-of-a-graph.md) $BC,CA,AD,DE,EA,AF$ are pairwise distinct, although $A$ occurs twice. Visiting a junction again and traversing a road segment again are different events.[Thomas Zaslavsky, Supplementary Notes for Graduate Graph Theory: trails and paths](https://people.math.binghamton.edu/zaslav/Oldcourses/581.S99/notes.html)

In an [undirected graph](undirected-graph.md), traversing $AB$ and then $BA$ repeats the same [edge](edge-of-a-graph.md); direction of travel does not give it a new identity. In a [multigraph](multigraph.md) with distinct parallel [edges](edge-of-a-graph.md) $p,q$ joining $X$ and $Y$, the [closed walk](closed-walk.md) $(X,p,Y,q,X)$ is a [trail](trail-in-a-graph.md), whereas $(X,p,Y,p,X)$ is not. Both have the same [vertex](vertex-graph-theory.md) [sequence](sequence.md) $X,Y,X$. In a [directed graph](directed-graph.md), separate [directed edges](directed-edge.md) $X\to Y$ and $Y\to X$ may instead be used once each; record their identities and obey their directions. Thus testing a [trail](trail-in-a-graph.md) means checking the actual [edge](edge-of-a-graph.md) records, not merely checking consecutive endpoint labels.

For a finite [graph](graph-split.md), a [trail](trail-in-a-graph.md) has length at most $|E|$; unrestricted [walks](walk-in-a-graph.md) can have arbitrarily large length whenever a positive-length [closed walk](closed-walk.md) exists, since it can be repeated. An [Eulerian trail](eulerian-trail.md) is the special [trail](trail-in-a-graph.md) that uses every [edge](edge-of-a-graph.md), so its length is exactly $|E|$. Our length-six [trail](trail-in-a-graph.md) omits $AB$ and is therefore not an [Eulerian trail](eulerian-trail.md). In a road-inspection model, a [trail](trail-in-a-graph.md) describes servicing its selected segments once while allowing returns to junctions; requiring service of every segment leads to the [Eulerian trail](eulerian-trail.md) question. If extra travel between serviced segments is necessary, the complete journey can be a [walk](walk-in-a-graph.md) even when each segment is serviced only once. This distinction keeps the service requirement separate from the route actually travelled.

## ↑ Ancestors (6)

1. [Walk in a graph](walk-in-a-graph.md)
2. [Graph theory](graph-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Eulerian trail](eulerian-trail.md)
