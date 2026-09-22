# 3-SAT reduction to vertex cover

↑ **Parent:** [Vertex cover](vertex-cover.md)

A [polynomial-time many-one reduction](polynomial-time-many-one-reduction.md) represents each variable by an adjacent literal pair and each clause by a [triangle in a graph](triangle-in-a-graph.md). Connect each occurrence vertex to its corresponding literal vertex. A [vertex cover](vertex-cover.md) of size $n+2m$ must choose one literal vertex per variable and two vertices per clause, and its omitted clause vertex forces a true literal. Conversely a satisfying [Boolean valuation](boolean-valuation.md) supplies such a cover. This establishes [NP-hardness](np-hardness.md) of the vertex-cover decision problem from [3-SAT](3-sat.md).

## ↑ Ancestors (6)

1. [Vertex cover](vertex-cover.md)
2. [Graph theory](graph-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
