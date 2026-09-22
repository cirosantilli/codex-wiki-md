<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Fix a root $r$. On a [recurrent graph](../../../../../../recurrent-graph.md), a [simple random walk](../../../../../../simple-random-walk.md) started at any vertex hits $r$ [almost surely](../../../../../../almost-sure-convergence.md). Run [Wilson's algorithm](../../../../../../wilson-s-algorithm.md) with root $r$: successively attach the [loop-erased random walk](../../../../../../loop-erased-random-walk.md) from each new starting vertex, stopped when it hits the existing tree. Every walk terminates [almost surely](../../../../../../almost-sure-convergence.md), because that tree already contains $r$.

To compare the two finite approximations, fix a finite set of edges $K$ and put all their endpoints first in the ordering of starting vertices. In the infinite [graph](../../../../../../graph-split.md), these finitely many [Wilson's algorithm](../../../../../../wilson-s-algorithm.md) walks have finite lengths [almost surely](../../../../../../almost-sure-convergence.md). Their visited vertices, together with their neighbors, are therefore contained in $V_k$ for all sufficiently large $k$ on each realization.

Couple the walks in $G[V_k]$, in $G_k^{\mathrm w}$, and in $G$ using the same neighbor choices while they are in the interior of $V_k$. On the event just described, they encounter neither boundary, so the walks, their chronological [loop erasures](../../../../../../loop-erasure.md), and the resulting partial trees agree. Once every endpoint of $K$ has entered the partial tree, later walks cannot add any edge of $K$: they stop on their first hit of the existing tree. Thus the indicators of membership for all edges of $K$ agree in the free and wired [uniform spanning trees](../../../../../../uniform-spanning-tree.md), with probability tending to one.

The two limiting measures agree on every finite-edge event, and therefore

$$
\boxed{\mathrm{WSF}=\mathrm{FSF}.}
$$

This argument also shows that the common [uniform spanning forest](../../../../../../uniform-spanning-forest.md) is a single spanning [tree](../../../../../../tree-graph-theory.md) on a [recurrent graph](../../../../../../recurrent-graph.md). The equality refers to probability measures, not to independently sampled forests being identical.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 214](../../../paper-214-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
