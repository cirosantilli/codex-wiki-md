<h1 id="a/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

An [edge loop](../../../../edge-loop.md) is a finite sequence of vertices $v_0,\ldots,v_m$, starting and ending at $b$, in which consecutive distinct vertices span an edge. Two such sequences are equivalent when related by finitely many elementary edge homotopies, with endpoints fixed: insert or delete a repeated vertex, cancel or insert a spur $(u,v,u)$, and replace $(u,v,w)$ by $(u,w)$ or conversely when the vertices lie in one [simplex](../../../../simplex.md). Repetitions are allowed in this last convention; a nondegenerate move uses a triangle.

The [edge-loop group](../../../../edge-loop-group.md) $E(K,b)$ consists of these equivalence classes, with product given by concatenating the sequences at $b$. Elementary moves remain valid inside a longer concatenation, so this product is well defined. Concatenation is associative after the harmless repeated base vertex is removed; the constant [edge loop](../../../../edge-loop.md) is the identity. Reversing a sequence gives its inverse, because a sequence followed by its reverse cancels by successive spurs. Thus these operations do form a group.

Realize an [edge loop](../../../../edge-loop.md) as a piecewise linear path in the [geometric realization](../../../../geometric-realization-of-a-simplicial-complex.md) $|K|$. A spur contracts in an edge, and a triangle move is a [homotopy](../../../../homotopy-split.md) across that triangle, always fixing endpoints. Hence realization gives a well-defined map $\theta$ to the [fundamental group](../../../../fundamental-group.md). Realization respects concatenation up to endpoint-preserving reparametrization, so $\theta$ is a [homomorphism](../../../../homomorphism.md).

The relative [Simplicial approximation theorem](../../../../simplicial-approximation-theorem.md) says that a continuous map from a finite complex to a [geometric realization](../../../../geometric-realization-of-a-simplicial-complex.md) is homotopic, after sufficiently fine subdivision of its domain, to a simplicial map, with a chosen already simplicial subcomplex kept fixed. Apply its based-[circle](../../../../circle.md) version to a loop, keeping its marked vertex at $b$. The resulting subdivided simplicial [circle](../../../../circle.md) traverses edges, so every [based homotopy](../../../../based-homotopy.md) class has an edge-loop representative. Thus **$\theta$ is surjective**.

For the full two-skeleton, use the triangles through $b$ to replace each edge $(u,v)$ of a loop by $(u,b,v)$. Degenerate cases use repeated-vertex or spur moves. The resulting path contracts by spurs, so its [edge-loop group](../../../../edge-loop-group.md), and therefore its [fundamental group](../../../../fundamental-group.md), is trivial. This also covers one or two vertices, when only repeated vertices and spurs are needed.

If the deleted triangle has vertices $u,v,w$, choose a fourth vertex $t$. Its boundary is filled by the three present triangles $(t,u,v)$, $(t,v,w)$ and $(t,w,u)$: their union is the cone from $t$ on that boundary. Every elementary [homotopy](../../../../homotopy-split.md) that formerly crossed the missing triangle can therefore be replaced by a [homotopy](../../../../homotopy-split.md) through these three triangles, staying in $|L|$. Since the one-skeleton has not changed, the same contraction of any [edge loop](../../../../edge-loop.md) is available in $L$. Surjectivity of its realization map gives

$$
\boxed{\pi_1(|K|,b)=1,\qquad\pi_1(|L|,b)=1\quad(n\geq4\text{ for }L)}.
$$

## ↑ Ancestors (12)

1. [1](../1.md)
2. [A](../../a.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the topology and Groups and Algebraic Topology course of the University of Oxford](../../../split.md)
5. [Topology and Groups and Algebraic Topology course of the University of Oxford](../../../../topology-and-groups-and-algebraic-topology-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
