<h1 id="prufer-degree-formula">Prüfer degree formula</h1>

↑ **Parent:** [Prüfer sequence](prufer-sequence.md)

For a [labelled tree](labelled-tree.md) with $n\geq2$ [vertices](vertex-graph-theory.md), the [vertex degree](degree-graph-theory.md) of label $v$ is one plus the number of occurrences of $v$ in its [Prüfer sequence](prufer-sequence.md):

$$
\deg_T(v)=1+\#\{i:p_i=v\}.
$$

Each recording of $v$ corresponds to an incident [edge](edge-of-a-graph.md) removed when a neighbouring [leaf of a graph](leaf-of-a-graph.md) is deleted. Exactly one incident [edge](edge-of-a-graph.md) remains when $v$ itself is deleted, or when it belongs to the final pair. In particular, $v$ is a [leaf of a graph](leaf-of-a-graph.md) exactly when it never occurs in the [Prüfer sequence](prufer-sequence.md). The same reasoning applies to each remaining [tree](tree-graph-theory-split.md) and its remaining code. [Columbia University, Graph Theory Lecture 4, Proposition 7.1: degree equals occurrences plus one](https://www.cs.columbia.edu/~cs4203/files/GT-Lec4.pdf)

For $p=(1,3,3,5)$, the occurrence counts in label order are $(1,0,2,0,1,0)$, giving the [degree sequence](degree-sequence.md) $(2,1,3,1,2,1)$. Its sum is $10=2(6-1)$, as required by the [degree-sum formula](degree-sum-formula.md). More generally, summing the occurrence counts gives $n-2$, so summing the [vertex degrees](degree-graph-theory.md) gives $n+(n-2)=2(n-1)$.

**Table of contents**

- [Labelled tree count with prescribed degrees](labelled-tree-count-with-prescribed-degrees.md)

## ↑ Ancestors (7)

1. [Prüfer sequence](prufer-sequence.md)
2. [Cayley's formula](cayley-s-formula.md)
3. [Tree (graph theory)](tree-graph-theory-split.md)
4. [Combinatorics](combinatorics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Labelled tree count with prescribed degrees](labelled-tree-count-with-prescribed-degrees.md)
- [Prüfer sequence](prufer-sequence.md)
- [Uniform labelled tree generation](uniform-labelled-tree-generation.md)
