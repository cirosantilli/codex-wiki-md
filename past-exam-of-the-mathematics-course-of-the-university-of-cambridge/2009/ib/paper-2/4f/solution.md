<h1 id="4f/solution">Solution</h1>

↑ **Parent:** [4F](../4f.md)

A [Hausdorff space](../../../../../hausdorff-space.md) is a [topological space](../../../../../topological-space.md) in which any two distinct points have disjoint open neighborhoods. Let $K$ be a [compact subset](../../../../../compact-space.md) of a [Hausdorff space](../../../../../hausdorff-space.md) and $x\notin K$. For each $y\in K$, choose disjoint open neighborhoods $U_y$ of $y$ and $W_y$ of $x$. The $U_y$ cover $K$, so [compactness](../../../../../compact-space.md) gives a finite subcover $U_{y_1},\ldots,U_{y_m}$. Their paired intersection $W=\bigcap_{r=1}^mW_{y_r}$ is an open neighborhood of $x$ disjoint from $K$. Thus every point of its complement has an open neighborhood in the complement, proving **every [compact subset of a Hausdorff space](../../../../../compact-subset-of-a-hausdorff-space.md) is closed**. The empty set case is immediate.

In the [cocountable topology](../../../../../countable-complement-topology.md) on an uncountable set, any two nonempty open sets intersect: their combined complements are countable and cannot exhaust $X$. Thus **the space is not [Hausdorff](../../../../../hausdorff-space.md)**.

Nevertheless **every [compact subset](../../../../../compact-space.md) is closed** here. In fact only finite subsets are compact. To prove this, suppose $K$ is infinite and choose distinct points $d_1,d_2,\ldots\in K$. The open sets

$$
U_n=X\setminus\{d_m:m\ge n\}
$$

form an increasing [open cover](../../../../../open-cover.md) of $X$, and hence of $K$. Any finite selection is contained in $U_N$ for its largest index $N$, which misses $d_N\in K$. So $K$ is not compact. Finite sets are compact in any [topological space](../../../../../topological-space.md), and in this [cocountable topology](../../../../../countable-complement-topology.md) they are closed because their complements are open. This proves the claimed behavior of [compact subsets of a cocountable space](../../../../../compact-subsets-of-a-cocountable-space.md).

## ↑ Ancestors (10)

1. [4F](../4f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
