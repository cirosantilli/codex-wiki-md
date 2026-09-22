<h1 id="3/c/ii/solution">Solution</h1>

↑ **Parent:** [ii](../ii.md)

Every complete [polygon edge](../../../../../side-of-a-polygon.md) pairing gives a [compact](../../../../../compact-space.md) [connected](../../../../../connected-space.md) [surface](../../../../../topological-surface-split.md) with empty [manifold boundary](../../../../../manifold-boundary.md). Here is the local reason at the vertices. Replace each [polygon](../../../../../polygon.md) corner by a small link [interval](../../../../../interval-mathematics.md). The [polygon edge](../../../../../side-of-a-polygon.md) pairings identify all endpoints of these link [intervals](../../../../../interval-mathematics.md) in pairs. In a given vertex [equivalence class](../../../../../equivalence-class.md), the resulting [graph](../../../../../graph-split.md) is [connected](../../../../../connected-space.md): the endpoint identifications generating that vertex [equivalence class](../../../../../equivalence-class.md) also connect its corner [intervals](../../../../../interval-mathematics.md). Every link [graph vertex](../../../../../vertex-graph-theory.md) has [degree of a vertex](../../../../../degree-graph-theory.md) two, so the [graph](../../../../../graph-split.md) is a [circle](../../../../../circle.md). Its [topological cone](../../../../../cone-topology.md) is a [disc](../../../../../topological-disc.md), giving the required local [surface](../../../../../topological-surface-split.md) model. Edge and face [CW cell](../../../../../topological-cell.md) interiors have the usual [disc](../../../../../topological-disc.md) [neighbourhoods](../../../../../neighbourhood-mathematics.md) as well. A finite [triangulation](../../../../../triangulation.md) compatible with the [polygon edge](../../../../../side-of-a-polygon.md) pairings realizes the result as a finite [simplicial complex](../../../../../simplicial-complex.md), giving a [Hausdorff](../../../../../hausdorff-space.md), [second-countable space](../../../../../second-countable-space.md).

For every such [surface](../../../../../topological-surface-split.md), $\chi=V-2\geq-1$. If it is [orientable](../../../../../orientable-surface.md), the [classification of compact surfaces](../../../../../classification-of-compact-surfaces.md) gives $\chi=2-2g$, so $g=0$ or $1$. If it is a [nonorientable surface](../../../../../non-orientable-surface.md), write $k\geq1$ for its [nonorientable genus](../../../../../nonorientable-genus.md); then $\chi=2-k\geq-1$ gives $k\leq3$. The exhaustive list is therefore

- the [sphere](../../../../../sphere.md) $S^2$;
- the [torus](../../../../../torus.md) $T^2$;
- the [real projective plane](../../../../../real-projective-plane.md) $\mathbb{RP}^2$;
- the [Klein bottle](../../../../../klein-bottle.md) $\mathbb{RP}^2\mathbin\#\mathbb{RP}^2$;
- the [connected sum of surfaces](../../../../../connected-sum-of-surfaces.md) $\mathbb{RP}^2\mathbin\#\mathbb{RP}^2\mathbin\#\mathbb{RP}^2$, a [nonorientable surface](../../../../../non-orientable-surface.md) of [nonorientable genus](../../../../../nonorientable-genus.md) three.

To prove that every listed possibility actually occurs, the following six-letter boundary words specify complete pairings of a [hexagon](../../../../../hexagon.md):

$$
\begin{array}{c|c|c|c}
\text{surface}&\text{boundary word}&V&\chi=V-2\\\hline
S^2&aa^{-1}bb^{-1}cc^{-1}&4&2\\
\mathbb{RP}^2&aabb^{-1}cc^{-1}&3&1\\
T^2&abca^{-1}b^{-1}c^{-1}&2&0\\
\text{Klein bottle}&aba^{-1}bcc^{-1}&2&0\\
\mathbb{RP}^2\#\mathbb{RP}^2\#\mathbb{RP}^2&aabbcc&1&-1
\end{array}
$$

The vertex counts follow by matching starts and ends of equally directed arrows, just as in part (b). The first and third words pair every letter with its inverse, giving [orientable](../../../../../orientable-surface.md) [surfaces](../../../../../topological-surface-split.md). Each other word contains a letter twice with the same sign, giving a [nonorientable surface](../../../../../non-orientable-surface.md): an [orientation](../../../../../orientation-of-a-simplex.md) on the face would induce equal, rather than opposite, boundary directions along that glued pair. With the displayed [Euler characteristics](../../../../../euler-characteristic.md), the [classification of compact surfaces](../../../../../classification-of-compact-surfaces.md) identifies the examples exactly as listed. **All five types occur, and no others occur.**

## ↑ Ancestors (13)

1. [ii](../ii.md)
2. [c](../../c.md)
3. [3](../../../3.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the topology course of the University of Oxford](../../../../split.md)
6. [Topology course of the University of Oxford](../../../../../topology-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
