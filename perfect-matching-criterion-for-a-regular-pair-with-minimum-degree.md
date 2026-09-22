# Perfect matching criterion for a regular pair with minimum degree

↑ **Parent:** [Regular pair of vertex sets](regular-pair-of-vertex-sets.md)

Let $(X,Y)$ be a [regular pair of vertex sets](regular-pair-of-vertex-sets.md) with parameter $\epsilon$, equal class sizes $n$, density greater than $\epsilon$, and every vertex having at least $\epsilon n$ neighbors across the pair. Then it has a [perfect matching](perfect-matching.md). To prove [Hall's condition](hall-s-marriage-theorem.md), take $S\subseteq X$. If $0<|S|\leq\epsilon n$, one vertex already supplies at least $|S|$ neighbors. If $\epsilon n<|S|\leq(1-\epsilon)n$ and $|N(S)|<|S|$, the two large sets $S$ and $Y\setminus N(S)$ have density zero, contradicting [regularity](regular-pair-of-vertex-sets.md) and the positive density surplus. Finally, if $|S|>(1-\epsilon)n$, every vertex of $Y$ has a neighbor in $S$, so $N(S)=Y$. The empty subset satisfies Hall's condition directly.

## ↑ Ancestors (8)

1. [Regular pair of vertex sets](regular-pair-of-vertex-sets.md)
2. [Edge density of a bipartite graph](edge-density-of-a-bipartite-graph.md)
3. [Probabilistic combinatorics](probabilistic-combinatorics-split.md)
4. [Graph theory](graph-theory-split.md)
5. [Foundations of mathematics](foundations-of-mathematics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford/2010/a/3/c/solution.md)
