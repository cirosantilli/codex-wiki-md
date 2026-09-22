<h1 id="1/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

We use the [uniqueness of the infinite percolation cluster](../../../../../../../uniqueness-of-the-infinite-percolation-cluster.md) on $\mathbb Z^d$: for $p>p_c$, there is [almost surely](../../../../../../../almost-sure-convergence.md) exactly one infinite [percolation cluster](../../../../../../../percolation-cluster.md), denoted $I$. Fix $m$ and let $N>m$. Two observations account for the possible distinct endpoints of the face connections.

First, the probability that some finite [percolation cluster](../../../../../../../percolation-cluster.md) meeting $B(m)$ reaches $\partial B(N)$ tends to zero as $N\to\infty$. There are only finitely many vertices in $B(m)$, and each of their finite [percolation clusters](../../../../../../../percolation-cluster.md) has finite radius; apply the [union bound](../../../../../../../boole-s-inequality.md) and [continuity from above of a measure](../../../../../../../continuity-from-above-of-a-measure.md).

Second, all vertices of $I\cap B(m)$ are joined to one another inside $B(N)$ with probability tending to one. On each configuration, this is a finite set of vertices of one connected [percolation cluster](../../../../../../../percolation-cluster.md). Choose a finite open [path in a graph](../../../../../../../path-in-a-graph.md) from one such vertex to each of the others; the union of these finitely many paths is contained in some finite box. The assertion is vacuous if the set is empty.

By part (b.ii), each of the two face-connection events within $B(N)$ fails with probability at most $\delta_m^{1/(2d)}$. Outside the two exceptional events just described, their endpoints in $B(m)$ belong to $I$ and can be joined inside $B(N)$. Concatenating the left-face path, that joining path, and the right-face path produces a crossing of $B(N)$. Consequently

$$
\limsup_{N\to\infty}\mathbb P_p(\mathrm{LR}(N)^c)\leq2\delta_m^{1/(2d)}.
$$

Now let $m\to\infty$. Since $\delta_m\to0$,

$$
\boxed{\lim_{N\to\infty}\mathbb P_p(\mathrm{LR}(N))=1.}
$$

The order of limits matters: $m$ is fixed while the finitely many relevant [percolation clusters](../../../../../../../percolation-cluster.md) are connected inside increasingly large boxes.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 214](../../../../paper-214-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
