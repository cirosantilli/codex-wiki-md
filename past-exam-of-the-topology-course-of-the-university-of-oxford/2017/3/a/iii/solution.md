<h1 id="3/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use a convex representative of the marked [polygonal schema](../../../../../polygonal-schema.md), retaining the side-pairing parametrizations. This does not change the quotient up to homeomorphism: a matching boundary homeomorphism extends over the two polygonal discs by radial extension in disc coordinates. Join an interior point to every vertex, producing finitely many triangles. Orient radial edges away from the interior point and choose boundary-edge orientations consistently with the side identifications. Each triangle then has a local vertex ordering with the centre first; the other two vertices are ordered along its boundary-edge arrow. These orderings agree on shared edges, so the quotient is a finite [delta-complex](../../../../../delta-complex.md) $X$ whose underlying space is the prescribed polygon quotient.

This need not yet be an [abstract simplicial complex](../../../../../simplicial-complex.md): two vertices of a triangle may become identified, or different triangles may have the same vertex set. Apply [barycentric subdivision](../../../../../barycentric-subdivision.md) twice.

In the first subdivision, every small simplex corresponds to a flag of faces of strictly increasing dimensions. Identifications preserve dimension, so its vertices are distinct. In the second subdivision, a vertex records an actual cell of the first subdivision. A set of such vertices determines their order by dimension. Inside any one first-subdivision simplex, distinct vertices make each face inclusion uniquely determined by its vertex subset; hence a flag has at most one realization. Therefore different second-subdivision simplexes cannot share the same vertex set, and they meet in precisely their common faces. Thus the second subdivision is an abstract simplicial complex $L$.

The affine subdivision maps are compatible with every face identification, so their realizations are homeomorphisms. Consequently

$$
\boxed{P/{\sim}\ \cong\ |X|\ \cong\ |L|,}
$$

where $L$ is finite. This proves [triangulation of a polygon with paired sides](../../../../../triangulation-of-a-polygon-with-paired-sides.md) by the [second barycentric subdivision of a delta-complex](../../../../../second-barycentric-subdivision-of-a-delta-complex.md) construction.[§2.1, exercise 23, p. 133: distinct vertices after one subdivision and a simplicial complex after two](../../../../../algebraic-topology-by-allen-hatcher.md)

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the topology course of the University of Oxford](../../../../split.md)
6. [Topology course of the University of Oxford](../../../../../topology-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
