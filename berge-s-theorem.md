<h1 id="berge-s-theorem">Berge's theorem</h1>

↑ **Parent:** [Augmenting path in a matching](augmenting-path-in-a-matching.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Berge's_theorem)

For a finite [simple graph](simple-graph.md) $G$ and a [matching in a graph](matching-graph-theory-split.md) $M\subseteq E(G)$, $M$ is a [maximum cardinality matching](maximum-cardinality-matching.md) if and only if $G$ has no [augmenting path in a matching](augmenting-path-in-a-matching.md) relative to $M$. The [graph](graph-split.md) need not be a [bipartite graph](bipartite-graph-split.md), and the assertion concerns [cardinality](cardinality.md), not edge benefits.[Claude Berge, Two theorems in graph theory, printed p. 842: finite unoriented graph and Problem 3; printed p. 843, Theorem 1: maximum matching and absence of an alternating chain between neutral points](two-theorems-in-graph-theory-by-claude-berge.md)

The criterion turns a global comparison with every competing [matching in a graph](matching-graph-theory-split.md) into a search for one repair. Starting from any [matching in a graph](matching-graph-theory-split.md), repeatedly find and toggle an [augmenting path in a matching](augmenting-path-in-a-matching.md). Each step adds one selected [edge](edge-of-a-graph.md), so finiteness gives termination after at most $\lfloor |V(G)|/2\rfloor-|M|$ steps; absence of any further [augmenting path in a matching](augmenting-path-in-a-matching.md) certifies maximum [cardinality](cardinality.md). This is an optimality criterion, not by itself a bound on the work needed to find each [graph path](path-in-a-graph.md).

For a short proof outline, an [augmenting path in a matching](augmenting-path-in-a-matching.md) immediately contradicts maximum [cardinality](cardinality.md). Conversely, if another [matching in a graph](matching-graph-theory-split.md) $N$ has $|N|>|M|$, consider the [subgraph](subgraph.md) whose [set](set-split.md) of [edges](edge-of-a-graph.md) is $M\mathbin\triangle N$. Its [vertices](vertex-graph-theory.md) have [degree of a vertex](degree-graph-theory.md) at most two; its nontrivial [connected components](connected-component.md) are [graph paths](path-in-a-graph.md) and even [cycles in a graph](cycle-in-a-graph.md), alternating between the two [matchings in a graph](matching-graph-theory-split.md). A [cycle in a graph](cycle-in-a-graph.md) contributes equal numbers from each. Hence some [graph path](path-in-a-graph.md) contributes one more [edge](edge-of-a-graph.md) from $N$ than from $M$ and starts and ends with [edges](edge-of-a-graph.md) from $N$. Its endpoints are [unmatched vertices in a matching](unmatched-vertex-in-a-matching.md) relative to $M$, yielding the required [augmenting path in a matching](augmenting-path-in-a-matching.md).

## ↑ Ancestors (7)

1. [Augmenting path in a matching](augmenting-path-in-a-matching.md)
2. [Matching (graph theory)](matching-graph-theory-split.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Matching (graph theory)](matching-graph-theory-split.md)
- [Maximum cardinality matching](maximum-cardinality-matching.md)
