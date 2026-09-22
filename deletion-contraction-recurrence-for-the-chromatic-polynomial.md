# Deletion-contraction recurrence for the chromatic polynomial

↑ **Parent:** [Chromatic polynomial](chromatic-polynomial.md)

Deleting an edge removes one colour constraint. [Edge contraction](edge-contraction.md) describes exactly the newly admitted colourings that violate that constraint. If $e$ joins distinct [vertices](vertex-graph-theory.md) $u,v$ of a [simple graph](simple-graph.md) $G$, write $G-e$ for the [graph](graph-split.md) with that [edge](edge-of-a-graph.md) deleted and $G/e$ for the [graph](graph-split.md) with $u,v$ identified and $e$ removed. Parallel edges produced by the contraction may be reduced to one edge, since they impose the same condition on a [proper vertex coloring](proper-vertex-coloring.md). Then

$$
P_G(t)=P_{G-e}(t)-P_{G/e}(t).
$$

To see why, divide the [proper vertex colorings](proper-vertex-coloring.md) of $G-e$ into two classes. Those with different colours at $u,v$ are exactly the colourings of $G$. Those with equal colours at $u,v$ correspond one-to-one to colourings of $G/e$: the merged [vertex](vertex-graph-theory.md) receives their common colour. Subtracting the second class leaves the first.

For the triangle, delete $AC$ to get a three-vertex [path graph](path-graph.md), or contract $AC$ to get two [vertices](vertex-graph-theory.md) joined by an [edge](edge-of-a-graph.md) after removing the redundant parallel edge. Consequently,

$$
P_{K_3}(t)=t(t-1)^2-t(t-1)=t(t-1)(t-2).
$$

At $t=3$, this says **$6=12-6$**. Of the twelve path colourings pictured above, six give $A,C$ the same colour; these are precisely the ones ruled out when we restore $AC$.

<a id="image-deleting-and-contracting-a-triangle-edge-separates-the-allowed-and-newly-forbidden-colourings"></a>
![](chromatic-polynomial-deletion-contraction.png)

**[Figure 8](#image-deleting-and-contracting-a-triangle-edge-separates-the-allowed-and-newly-forbidden-colourings). Deleting and contracting a triangle edge separates the allowed and newly forbidden colourings**.

This recurrence is useful because it reduces a constrained counting problem to smaller [graphs](graph-split.md). A [graph](graph-split.md) on $n$ [vertices](vertex-graph-theory.md) with no [edges](edge-of-a-graph.md) has $P_G(t)=t^n$, since every [vertex](vertex-graph-theory.md) chooses its colour independently. Repeated [edge](edge-of-a-graph.md) deletion and [edge contraction](edge-contraction.md) reduce to this case and show that the counting function is a [polynomial](polynomial-split.md). The same recurrence gives its leading coefficients. The method is conceptually simple, although the number of recursive cases can still grow rapidly.

## ↑ Ancestors (7)

1. [Chromatic polynomial](chromatic-polynomial.md)
2. [Graph coloring](graph-coloring-split.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-3/17f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-2/17h/a/solution.md)
