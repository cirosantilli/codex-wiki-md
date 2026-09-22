# Subset dynamic programming for a Hamiltonian path

↑ **Parent:** [Dynamic programming](dynamic-programming.md)

For a [directed graph](directed-graph.md) with [adjacency matrix](adjacency-matrix.md) $A$, let $D[S,v]$ record whether a path visits precisely the [vertices](vertex-graph-theory.md) of $S$ once and ends at $v$. The singleton states are true. A larger state is true exactly when some predecessor $u\in S\setminus\{v\}$ has a true state for $S\setminus\{v\}$ and an edge to $v$. Removing or adjoining the last edge proves this recurrence by [mathematical induction](mathematical-induction.md) on $|S|$. There are $n2^{n-1}$ states, each requiring at most $n-1$ predecessor checks, giving $O(n^22^n)$ time and $O(n2^n)$ storage. A true state for $S=V$ certifies a [Hamiltonian path](hamiltonian-path.md).

## ↑ Ancestors (5)

1. [Dynamic programming](dynamic-programming.md)
2. [Mathematical optimization](mathematical-optimization-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/functional-programming-design-and-analysis-of-algorithms/6/b/solution.md)
