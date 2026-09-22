<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Each factor is a [free abelian group](../../../../../../free-abelian-group.md) of rank two. Take the infinite symmetric generating set

$$
\boxed{S=(A\setminus\{1\})\cup(B\setminus\{1\}).}
$$

The [Bass-Serre tree](../../../../../../bass-serre-tree.md) has an edge $e_g$ joining $gA$ to $gB$ for every $g\in A*B$. Indeed, the [normal form theorem for a free product](../../../../../../normal-form-theorem-for-a-free-product.md) gives $A\cap B=\{1\}$, so a nonempty coset intersection consists of exactly one element. Let $m_g$ be the midpoint of $e_g$ and send the Cayley vertex $g$ to $m_g$.

Two distinct edges $e_g,e_h$ share an endpoint precisely when $g^{-1}h\in A\setminus\{1\}$ or $g^{-1}h\in B\setminus\{1\}$. This is exactly adjacency in the [Cayley graph](../../../../../../cayley-graph.md) for $S$. A path in that graph therefore gives a path between the midpoints of the same length in the tree. Conversely, the unique tree segment between two edge midpoints passes through a succession of adjacent edges and gives a Cayley path of that length. Hence, on vertices,

$$
\boxed{d_S(g,h)=d_{\mathcal T}(m_g,m_h).}
$$

All edge midpoints occur, and every tree point is within $1/2$ of one of them. Extending along Cayley edges gives a [quasi-isometry](../../../../../../quasi-isometry.md) of the metric graphs; ambiguity from folding the cliques at a tree vertex costs only a bounded additive error. This is the [free product with factor generating set](../../../../../../free-product-with-factor-generating-set.md) construction.

For finite generating sets the answer changes. Use $S_0=\{a,a',b,b'\}^{\pm1}$. The retraction $A*B\to A$ killing $B$ sends every generator to a generator of $A$ or to the identity. Therefore the restriction of $d_{S_0}$ to $A$ is exactly the standard $\ell^1$ [word metric](../../../../../../word-metric.md) on $\mathbb Z^2$.

In this grid, take vertices $(0,0),(2N,0),(0,2N)$. Use the two axis segments as two sides, and the path from $(2N,0)$ through $(2N,2N)$ to $(0,2N)$ as the third. All are [metric geodesics](../../../../../../metric-geodesic.md) in the whole [Cayley graph](../../../../../../cayley-graph.md), by the retraction argument. The corner $(2N,2N)$ is at distance $2N$ from either of the other sides. These [metric geodesic triangles](../../../../../../metric-geodesic-triangle.md) are arbitrarily thick, so this [Cayley graph](../../../../../../cayley-graph.md) is not a [Gromov-hyperbolic metric space](../../../../../../hyperbolic-metric-space.md).

A tree is $0$-hyperbolic. [Hyperbolicity is invariant under quasi-isometry](../../../../../../hyperbolicity-is-invariant-under-quasi-isometry.md) for [metric geodesic](../../../../../../metric-geodesic.md) spaces, and all finite [word metrics](../../../../../../word-metric.md) on this group are equivalent. Consequently **no [Cayley graph](../../../../../../cayley-graph.md) for a finite generating set is quasi-isometric to any tree**, including a locally infinite one.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 133](../../../paper-133-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
