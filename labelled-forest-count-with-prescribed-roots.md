# Labelled forest count with prescribed roots

↑ **Parent:** [Cayley's formula](cayley-s-formula.md)

For a fixed set of $k<n$ roots among $n$ labelled [vertices](vertex-graph-theory.md), the number of [forests](forest.md) with exactly one root in each [graph component](component-graph-theory.md) is $kn^{n-k-1}$. Orient edges toward their roots. Repeatedly remove the smallest nonroot leaf and record its parent. This gives a code of length $n-k$ whose last entry is a root. Conversely, for any such code choose the smallest remaining nonroot absent from the remaining code, join it to the first entry, and delete it. There is always a choice because the final entry is a root. These inverse operations give $n^{n-k-1}$ choices for the earlier entries and $k$ for the last. For $k=n$, the empty forest is unique.

## ↑ Ancestors (6)

1. [Cayley's formula](cayley-s-formula.md)
2. [Tree (graph theory)](tree-graph-theory.md)
3. [Combinatorics](combinatorics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Labelled unicyclic graph count](labelled-unicyclic-graph-count.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-12/4/i/solution.md)
