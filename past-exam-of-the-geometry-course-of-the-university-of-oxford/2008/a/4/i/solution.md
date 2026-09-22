<h1 id="a/4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a positively oriented curvilinear polygon bounding a disk $D$ in one coordinate patch, with exterior turning angles $\theta_i$, the [Gauss-Bonnet theorem](../../../../../gauss-bonnet-theorem.md) states

$$
\boxed{\int_DK\,dA+\int_{\partial D}\kappa_g\,ds+\sum_i\theta_i=2\pi.}
$$

For a closed compact [surface](../../../../../topological-surface-split.md) the global formula is

$$
\boxed{\int_SK\,dA=2\pi\chi(S).}
$$

Triangulate the [surface](../../../../../topological-surface-split.md) with each triangle contained in a coordinate patch. For each face, writing its exterior angles as $\pi$ minus its interior angles gives $\int K+\int\kappa_g=\sum\text{interior angles}-\pi$. On summing, the two contributions on each internal edge cancel, and all angles at each vertex sum to $2\pi$. Thus $\int_SK=2\pi V-\pi F$. Since $3F=2E$, this equals $2\pi(V-E+F)$, as required. For a [nonorientable surface](../../../../../non-orientable-surface.md) apply the [orientable](../../../../../orientable-surface.md) version to its [orientation double cover](../../../../../orientation-double-cover.md): both the curvature integral and [Euler characteristic](../../../../../euler-characteristic.md) double. With boundary, the same summation retains the boundary [geodesic](../../../../../geodesic.md)-curvature integral and the exterior angles at boundary corners, giving the corresponding global boundary formula with right side $2\pi\chi(S)$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [4](../../4.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the geometry course of the University of Oxford](../../../../split.md)
6. [Geometry course of the University of Oxford](../../../../../geometry-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
