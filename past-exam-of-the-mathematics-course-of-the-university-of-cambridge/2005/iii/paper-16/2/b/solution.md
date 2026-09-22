<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [compact metric space](../../../../../../compact-metric-space.md) is [second countable](../../../../../../second-countable-space.md). To see this concretely, for each positive integer $r$ choose a finite cover by balls of radius $1/r$. Their centres, over all $r$, form a countable [dense subset](../../../../../../dense-set.md); balls centred there with positive rational radii form a countable [basis of a topology](../../../../../../basis-of-a-topology.md). Enumerate its nonempty members as $(V_j)_{j\geq1}$, repeating members if the basis is finite.

For each $j$, put

$$
G_j=\bigcup_{n\geq1}f^{-n}(V_j).
$$

Each $G_j$ is an [open set](../../../../../../open-set.md), because all [iterations of a map](../../../../../../iterated-function.md) $f^n$ are [continuous](../../../../../../continuous-function.md). It is [dense](../../../../../../dense-set.md): if $U$ is any nonempty [open set](../../../../../../open-set.md), the hypothesis supplies $n\geq1$ and $u\in U$ with $f^n(u)\in V_j$, so $u\in U\cap G_j$.

A [compact metric space](../../../../../../compact-metric-space.md) is a [complete metric space](../../../../../../complete-metric-space.md), hence a [Baire space](../../../../../../baire-space.md). The [Baire category theorem](../../../../../../baire-category-theorem.md) implies that $G=\bigcap_{j\geq1}G_j$ is [dense](../../../../../../dense-set.md), and in particular nonempty. For any $x\in G$, the forward [orbit](../../../../../../orbit-dynamical-system.md) of $x$ meets every $V_j$, and therefore every nonempty [open set](../../../../../../open-set.md). Its [orbit closure](../../../../../../orbit-closure.md) is $X$. Thus **the open-set intersection hypothesis implies point transitivity**, and in fact the set of points with a dense forward [orbit](../../../../../../orbit-dynamical-system.md) contains the dense intersection $G$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
