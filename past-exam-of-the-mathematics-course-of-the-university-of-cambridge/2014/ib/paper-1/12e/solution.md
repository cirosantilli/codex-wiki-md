<h1 id="12e/solution">Solution</h1>

↑ **Parent:** [12E](../12e.md)

A [compact space](../../../../../compact-space.md) is one for which every [open cover](../../../../../open-cover.md) has a finite subcover. A [Hausdorff space](../../../../../hausdorff-space.md) has disjoint open neighbourhoods of any two distinct points.

Let $K$ be a compact subspace of a Hausdorff space $X$, and let $x\notin K$. For each $y\in K$, choose disjoint open neighbourhoods $U_y$ of $y$ and $V_y$ of $x$. Finitely many $U_{y_1},\ldots,U_{y_m}$ cover $K$. Their corresponding intersection $V_{y_1}\cap\cdots\cap V_{y_m}$ is an open neighbourhood of $x$ disjoint from $K$. Thus $X\setminus K$ is open, proving **compact subspaces of a Hausdorff space are closed**.

In particular, $C_1\cap C_2$ is closed as a subspace of compact $C_1$. A closed subset of a compact space is compact: add its open complement to an open cover, apply compactness to the whole space, and discard that extra open set. Hence **$C_1\cap C_2$ is compact**.

In the [cocountable topology](../../../../../countable-complement-topology.md) on $\mathbb R$, two nonempty open sets always intersect. Their two countable complements have countable union, which cannot exhaust the uncountable real line. Therefore **this space is not Hausdorff**.

Every finite subset is compact in any topology. Conversely, from any infinite subset $C$ select distinct points $c_1,c_2,\ldots$ and define

$$
U_n=\mathbb R\setminus\{c_j:j\geq n\}.
$$

Each $U_n$ is cocountable and open; the sets increase and their union is all of $\mathbb R$. They therefore cover $C$, but a finite selection is contained in some $U_N$, which misses the infinitely many $c_j$ with $j\geq N$. No finite subcover exists. Thus the [compact subsets of a cocountable space](../../../../../compact-subsets-of-a-cocountable-space.md) are

$$
\boxed{\text{exactly the finite subsets}.}
$$

## ↑ Ancestors (10)

1. [12E](../12e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
