# Cyclic successor colorings of regular graphs

↑ **Parent:** [Lovász local lemma](lovasz-local-lemma.md)

For each fixed integer $q\ge2$, every sufficiently high-degree finite regular [graph](graph-split.md) has an assignment of $q$ colors such that every vertex has a neighbour whose color is its successor modulo $q$. This assignment need not be a [proper vertex coloring](proper-vertex-coloring.md). If the degree is $r$, independent uniform vertex colors make a given vertex fail with probability $(1-1/q)^r$. That event depends on its closed neighbourhood, and has at most $r^2$ dependencies, since only centres within distance two matter. The symmetric [Lovász local lemma](lovasz-local-lemma.md) therefore gives such an assignment whenever $e(r^2+1)(1-1/q)^r\le1$, which holds for all sufficiently large $r$.

Choose one successor neighbour from each vertex. The resulting directed graph has outdegree one and hence contains a directed cycle. Its color increases once modulo $q$ on each step, so its length is divisible by $q$. Thus a nontrivial cycle of length a multiple of $q$ is obtained when $q\ge3$; for $q=2$ a directed two-cycle may simply traverse one undirected edge twice, so this last cycle inference needs a separate argument if an undirected simple cycle is required.

## ↑ Ancestors (7)

1. [Lovász local lemma](lovasz-local-lemma.md)
2. [Probabilistic combinatorics](probabilistic-combinatorics-split.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford/2007/b/5/b/solution.md)
