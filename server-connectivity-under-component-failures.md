# Server connectivity under component failures

↑ **Parent:** [Maximum flow problem](maximum-flow-problem.md)

To find the smallest link failure set separating a client from every server, add a common sink with sufficiently large-capacity server arcs and give original links unit capacities in both directions. The [max-flow min-cut theorem](max-flow-min-cut-theorem.md) identifies the minimum failure count $\lambda$. Unit-capacity [vertex splitting](vertex-splitting.md) also charges intermediary node failures. The network tolerates fewer than $\lambda$ failures and fails for some set of $\lambda$ failures. This concerns connection to at least one server, not separate connectivity to each server.

## ↑ Ancestors (7)

1. [Maximum flow problem](maximum-flow-problem.md)
2. [Flow network](flow-network.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-37/3/a/solution.md)
