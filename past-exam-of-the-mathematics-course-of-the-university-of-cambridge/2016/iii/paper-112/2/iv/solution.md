<h1 id="2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Choose a maximal subset $U\subset S^{n-1}$ whose distinct points have [Euclidean distance](../../../../../../euclidean-distance.md) greater than one. The [volumetric bound for Euclidean metric nets](../../../../../../volumetric-bound-for-euclidean-metric-nets.md) makes the construction finite: the open [Euclidean balls](../../../../../../euclidean-ball.md) of radius $1/2$ about the points of $U$ are disjoint and all lie in $(3/2)B^n$, so

$$
|U|\,2^{-n}v_n\leq(3/2)^nv_n,\qquad |U|\leq3^n.
$$

Maximality means that $U$ is a [metric net](../../../../../../metric-net.md) of radius one on the [unit sphere](../../../../../../unit-sphere.md). Thus every $\theta\in S^{n-1}$ has some $u\in U$ with $\lVert u-\theta\rVert\leq1$. Since both are [unit vectors](../../../../../../unit-vector.md),

$$
u\cdot\theta=1-\frac12\lVert u-\theta\rVert^2\geq\frac12.
$$

Now intersect the corresponding [closed half-spaces](../../../../../../closed-half-space.md):

$$
\boxed{P=\bigcap_{u\in U}\{x:u\cdot x\leq1/2\}.}
$$

The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) shows that $(1/2)B^n\subset P$. Conversely, write any nonzero $x\in P$ as $x=t\theta$ and choose $u$ as above. Then $t/2\leq t(u\cdot\theta)=u\cdot x\leq1/2$, so $t\leq1$. Hence $P\subset B^n$, which also proves boundedness. This [convex polytope](../../../../../../convex-polytope.md) has at most $|U|\leq3^n$ [facets](../../../../../../facet.md), since redundant inequalities can only reduce their number. **It meets the required inclusions with $r=2$.**

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [2](../../2.md)
3. [Paper 112](../../../paper-112-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
