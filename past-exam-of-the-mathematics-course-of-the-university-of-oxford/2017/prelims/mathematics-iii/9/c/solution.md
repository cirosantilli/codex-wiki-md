<h1 id="9/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Sort the distinct observations as $x_{(1)}<\cdots<x_{(n)}$. For ordered centres $m_1<\cdots<m_r$, a point is closer to $m_j$ than to $m_{j+1}$ precisely when it lies to the left of their midpoint. Thus each [Voronoi cell](../../../../../../voronoi-cell.md) is an [interval](../../../../../../interval-mathematics.md), with either choice allowed for an endpoint tie. Consequently, after assignment, each nonempty cluster is a contiguous block of the sorted observations.

The [arithmetic means](../../../../../../arithmetic-mean.md) of disjoint ordered blocks are strictly ordered, so updating centres preserves this order. The empty-cluster repair in part (b) preserves contiguous blocks too: an observation farthest from its assigned centre lies at an endpoint of its block, and removing that endpoint makes a new singleton block. In one dimension with distinct observations, choosing $K$ distinct observations as initial centres makes the first assignment nonempty.

The [one-dimensional K-means iteration bound](../../../../../../one-dimensional-k-means-iteration-bound.md) now follows by counting block partitions. Choosing the $K-1$ gaps between consecutive nonempty blocks gives

$$
\binom{n-1}{K-1}\le n^{K-1}
$$

possibilities. By the strict-decrease argument in part (b), no such partition can recur before [algorithm termination](../../../../../../algorithm-termination.md). Counting a step as an assignment, any empty-cluster repairs, and a centre update, with the stability check performed after that update, gives

$$
\boxed{\text{number of steps}\le\binom{n-1}{K-1}\le n^{K-1}.}
$$

For $K=1$, one update to the overall [arithmetic mean](../../../../../../arithmetic-mean.md) suffices. Arbitrary changes between tied centres would invalidate the strict-decrease argument, which is why the stable tie convention in part (b) matters.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [9](../../9.md)
3. [Mathematics III](../../../mathematics-iii-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
