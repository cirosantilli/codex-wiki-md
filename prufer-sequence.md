<h1 id="prufer-sequence">Prüfer sequence</h1>

↑ **Parent:** [Cayley's formula](cayley-s-formula.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Prüfer_sequence)

For $n\geq2$, a [Prüfer sequence](prufer-sequence.md) is the encoding of a [labelled tree](labelled-tree.md) on $\{1,\ldots,n\}$ by a [sequence](sequence.md)

$$
p=(p_1,\ldots,p_{n-2})\in\{1,\ldots,n\}^{n-2}.
$$

Repeated labels are allowed, and their order matters. To encode the [tree](tree-graph-theory.md), repeatedly remove its smallest-labelled [leaf of a graph](leaf-of-a-graph.md) together with its incident [edge](edge-of-a-graph.md), recording the label of its unique neighbour. Stop when two [vertices](vertex-graph-theory.md) remain; do not record their final [edge](edge-of-a-graph.md). Removing a [leaf of a graph](leaf-of-a-graph.md) leaves a [tree](tree-graph-theory.md), so the procedure makes exactly $n-2$ deletions. The choice of the smallest label makes the encoding deterministic. [Peter Magyar, Math 481: Prüfer encoding with the smallest leaf](https://users.math.msu.edu/users/magyarp/math481/)

For a concrete example, take six [vertices](vertex-graph-theory.md) and the set of [edges](edge-of-a-graph.md)

$$
E=\bigl\{\{1,2\},\{1,3\},\{3,4\},\{3,5\},\{5,6\}\bigr\}.
$$

Initially $2,4,6$ label the [vertices](vertex-graph-theory.md) of [vertex degree](degree-graph-theory.md) one. Remove $2$ and record its neighbour $1$. Now $1$ has become a [leaf of a graph](leaf-of-a-graph.md), so remove $1$ and record $3$. Next remove $4$ and record $3$ again; then remove $3$ and record $5$. The final [edge](edge-of-a-graph.md) joins $5$ and $6$. Thus the [Prüfer sequence](prufer-sequence.md) is

$$
p=(1,3,3,5).
$$

The deletion order is $2,1,4,3$: removing a [leaf of a graph](leaf-of-a-graph.md) can make its neighbour a [leaf of a graph](leaf-of-a-graph.md), so the eligible labels change as the [tree](tree-graph-theory.md) shrinks.

<a id="image-encoding-a-six-vertex-tree-as-the-prufer-sequence-1-3-3-5-then-reconstructing-its-five-edges"></a>
![](pruefer-tree-encoding.png)

**[Figure 12](#image-encoding-a-six-vertex-tree-as-the-prufer-sequence-1-3-3-5-then-reconstructing-its-five-edges). Encoding a six-vertex tree as the Prüfer sequence $(1,3,3,5)$, then reconstructing its five edges**.

To decode, keep a set $L$ of remaining labels, initially $\{1,\ldots,n\}$, and the remaining [sequence](sequence.md), initially $p$. While the [sequence](sequence.md) is nonempty, let $v$ be the smallest label in $L$ absent from the entire remaining [sequence](sequence.md). Add an [edge](edge-of-a-graph.md) between $v$ and its first entry, then remove $v$ from $L$ and delete that first entry. Finally join the two labels left in $L$. For the example:

| Remaining [sequence](sequence.md) before the step | Smallest absent remaining label | [Edge](edge-of-a-graph.md) added |
| --- | --- | --- |
| $(1,3,3,5)$ | $2$ | $\{2,1\}$ |
| $(3,3,5)$ | $1$ | $\{1,3\}$ |
| $(3,5)$ | $4$ | $\{4,3\}$ |
| $(5)$ | $3$ | $\{3,5\}$ |
| Empty; $L=\{5,6\}$ | Final pair | $\{5,6\}$ |

The decoder always has a choice: if the remaining [sequence](sequence.md) has length $m$, then $L$ has $m+2$ labels, so at least two of them are absent. Its first entry is still in $L$, and differs from the chosen absent label. Every removed [vertex](vertex-graph-theory.md) attaches to a [vertex](vertex-graph-theory.md) that survives longer; following these attachments eventually reaches the final pair. Consequently the decoded [graph](graph-split.md) is connected, and its $n-1$ [edges](edge-of-a-graph.md) make it a [tree](tree-graph-theory.md). In this construction, each occurrence of $v$ contributes an incident [edge](edge-of-a-graph.md), and $v$ gets one more [edge](edge-of-a-graph.md) at its final attachment. Thus a remaining label is absent from the remaining [sequence](sequence.md) exactly when it labels a [leaf of a graph](leaf-of-a-graph.md). Encoding and decoding choose the same smallest label at each step and undo each other. This [bijection](bijection.md) proves [Cayley's formula](cayley-s-formula.md) and explains why every freely chosen [sequence](sequence.md) is valid. [Columbia University, Graph Theory Lecture 4: Prüfer degree identity, decoding algorithm, and bijection](https://www.cs.columbia.edu/~cs4203/files/GT-Lec4.pdf)

For $n=2$ there is exactly one empty [sequence](sequence.md), and decoding adds the sole [edge](edge-of-a-graph.md). For $n=1$ there is one [tree](tree-graph-theory.md), with [vertex degree](degree-graph-theory.md) zero, but no length-$n-2$ [Prüfer sequence](prufer-sequence.md). This is the exception both to the encoding convention and to the [Prüfer degree formula](prufer-degree-formula.md).

Heinz Prüfer's 1918 paper "Neuer Beweis eines Satzes über Permutationen" appeared in Archiv der Mathematik und Physik, third series, volume 27, pages 142–144. It gives an encoding proof of the labelled [tree](tree-graph-theory.md) count. The historical title means "New proof of a theorem on permutations"; the modern [Prüfer sequence](prufer-sequence.md) permits repeated labels, so it is not a [permutation](permutation.md). [Prüfer (1918), original opening-page scan, page 142](https://i.sstatic.net/WDvxyMwX.png)

**Table of contents**

- [Prüfer degree formula](prufer-degree-formula.md)
  - [Labelled tree count with prescribed degrees](labelled-tree-count-with-prescribed-degrees.md)
- [Uniform labelled tree generation](uniform-labelled-tree-generation.md)

## ↑ Ancestors (6)

1. [Cayley's formula](cayley-s-formula.md)
2. [Tree (graph theory)](tree-graph-theory.md)
3. [Combinatorics](combinatorics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Cayley's formula](cayley-s-formula.md)
- [Prüfer degree formula](prufer-degree-formula.md)
- [Prüfer sequence](prufer-sequence.md)
- [Uniform labelled tree generation](uniform-labelled-tree-generation.md)
