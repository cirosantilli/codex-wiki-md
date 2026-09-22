# Three-edge path decomposition from a perfect matching

↑ **Parent:** [Cubic graph](cubic-graph.md)

A finite [simple graph](simple-graph.md) that is a [cubic graph](cubic-graph.md) and has a [perfect matching](perfect-matching.md) admits a [partition of a set](partition-of-a-set.md) of its [edges](edge-of-a-graph.md) into [graph paths](path-in-a-graph.md) of length three.

**Proof.** Delete a [perfect matching](perfect-matching.md) $M$. The remaining spanning [subgraph](subgraph.md) has [vertex degree](degree-graph-theory.md) two at every [vertex](vertex-graph-theory.md), so it consists of disjoint [graph cycles](cycle-in-a-graph.md). Orient each cyclically, giving a successor [bijection](bijection.md) $s$. Replace each $uv\in M$ by the [graph path](path-in-a-graph.md) $s(u),u,v,s(v)$. The four [vertices](vertex-graph-theory.md) are distinct: the successor [edges](edge-of-a-graph.md) are not in $M$, neither is a [self-loop](loop-graph-theory.md), and injectivity of $s$ excludes $s(u)=s(v)$. Every [edge](edge-of-a-graph.md) of $M$ appears once in the middle, and every other [edge](edge-of-a-graph.md) appears once at its unique tail. Thus the [graph paths](path-in-a-graph.md) cover every [edge](edge-of-a-graph.md) exactly once. In particular, the [perfect matching theorem for a cubic graph with at most two bridges](perfect-matching-theorem-for-a-cubic-graph-with-at-most-two-bridges.md) guarantees this decomposition under its hypotheses.

## ↑ Ancestors (7)

1. [Cubic graph](cubic-graph.md)
2. [Graph](graph-split.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2023/combinatorial-optimisation/3/b/ii/solution.md)
