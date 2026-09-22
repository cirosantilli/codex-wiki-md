<h1 id="13b/solution">Solution</h1>

↑ **Parent:** [13B](../13b.md)

The [product topology](../../../../../product-topology.md) on $X\times Y$ consists of arbitrary unions of rectangles $U\times V$ with $U\subseteq X$, $V\subseteq Y$ open. Such rectangles form a [basis of a topology](../../../../../basis-of-a-topology.md): every point lies in one, and intersections of two rectangles are rectangles with open factors.

If $d_X,d_Y$ induce the factor topologies, set

$$
\boxed{d((x,y),(x',y'))=\max\{d_X(x,x'),d_Y(y,y')\}.}
$$

Definiteness and symmetry are immediate. Each factor [triangle inequality](../../../../../triangle-inequality.md) bounds its distance by the sum of the two relevant product distances; taking the maximum proves the product [triangle inequality](../../../../../triangle-inequality.md). A ball of radius $r$ is exactly $B_X(x,r)\times B_Y(y,r)$, so every metric-open set is product-open. Conversely an open rectangle containing $(x,y)$ contains a product ball with radius the minimum of two suitable factor radii. Hence the [maximum product metric](../../../../../maximum-product-metric.md) induces precisely the [product topology](../../../../../product-topology.md).

A [compact space](../../../../../compact-space.md) is one for which every [open cover](../../../../../open-cover.md) has a finite subcover. Let $\mathcal U$ cover $X\times Y$, with both factors compact; if either is empty the result is immediate. For each fixed $x$ and each $y$, choose a rectangle $U_{x,y}\times V_{x,y}$ containing $(x,y)$ and lying in a member of $\mathcal U$. The sets $V_{x,y}$ cover $Y$, so finitely many, indexed by $y_1,\ldots,y_{m_x}$, suffice. Their $X$-neighbourhoods have open intersection

$$
U_x=\bigcap_{j=1}^{m_x}U_{x,y_j},
$$

containing $x$. The finitely many selected members of $\mathcal U$ cover all of $U_x\times Y$. Now the sets $U_x$ cover $X$, so select finitely many of these by compactness of $X$. Taking the union of their finite selections from $\mathcal U$ gives a finite cover of the whole product. **The product of two compact spaces is compact**, without requiring the factors to be Hausdorff.

## ↑ Ancestors (10)

1. [13B](../13b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
