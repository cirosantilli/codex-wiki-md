# Chromatic index bounds

↑ **Parent:** [Chromatic index](chromatic-index.md)

For every finite [simple graph](simple-graph.md), [Vizing's theorem](vizing-s-theorem.md) gives

$$
\Delta(G)\leq\chi\prime(G)\leq\Delta(G)+1.
$$

Here $\Delta(G)$ is the [maximum degree of a graph](maximum-degree-of-a-graph.md), taken as zero when there are no [vertices](vertex-graph-theory.md). A [bipartite graph](bipartite-graph-split.md) has the stronger equality $\chi\prime(G)=\Delta(G)$. The six-job [complete bipartite graph](complete-bipartite-graph.md) above attains this lower bound, while the [triangle in a graph](triangle-in-a-graph.md) attains the extra-colour alternative. The simple-[graph](graph-split.md) restriction in the upper bound matters.[Colouring, author-hosted chapter preview, §5.3, p. 132: Proposition 5.3.1 and Theorem 5.3.2](graph-theory-by-reinhard-diestel.md)

The [bipartite graph](bipartite-graph-split.md) equality still holds for finite loopless [multigraphs](multigraph.md), with parallel [edges](edge-of-a-graph.md) counted separately in each [vertex degree](degree-graph-theory.md). For instance, $r$ parallel jobs between two resources need exactly $r$ slots: every pair conflicts, and $\Delta=\chi\prime=r$. For a general finite loopless [multigraph](multigraph.md), however, the [simple graph](simple-graph.md) upper bound can fail. Put two parallel [edges](edge-of-a-graph.md) on each side of a [triangle in a graph](triangle-in-a-graph.md). All six [edges](edge-of-a-graph.md) pairwise share a [vertex](vertex-graph-theory.md), so each needs its own colour; every [vertex](vertex-graph-theory.md) has [degree of a vertex](degree-graph-theory.md) four. Consequently $\chi\prime=6>\Delta+1=5$. A multiplicity-aware bound is $\chi\prime(G)\leq\Delta(G)+\mu(G)$, where $\mu(G)$ is the largest number of parallel [edges](edge-of-a-graph.md) between a pair of [vertices](vertex-graph-theory.md). The doubled [triangle in a graph](triangle-in-a-graph.md) has $\mu=2$ and attains that bound. These statements exclude [self-loops](loop-graph-theory.md); the two-distinct-resource scheduling model excludes them too.[Line graphs and edge coloring, slide 2: bipartite multigraph equality, multiplicity bound and fat triangle](line-graphs-and-edge-coloring.md)

For historical orientation, [Graph Theory by Reinhard Diestel](graph-theory-by-reinhard-diestel.md) (Colouring preview, §5.3, p. 132) dates the bipartite equality to 1916 and [Vizing's theorem](vizing-s-theorem.md) to 1964. These are textbook attributions; the original papers have not been inspected here. The results state existence of optimal or nearly optimal [proper edge colourings](proper-edge-coloring.md), rather than saying that arbitrary greedy choices will find them. The [list-chromatic index](list-chromatic-index.md) asks the further question of success for every sufficiently large family of allowed-colour lists.

## ↑ Ancestors (8)

1. [Chromatic index](chromatic-index.md)
2. [Edge coloring](edge-coloring.md)
3. [Graph coloring](graph-coloring-split.md)
4. [Graph theory](graph-theory-split.md)
5. [Foundations of mathematics](foundations-of-mathematics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
