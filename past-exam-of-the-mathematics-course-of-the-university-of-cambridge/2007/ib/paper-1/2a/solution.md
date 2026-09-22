<h1 id="2a/solution">Solution</h1>

↑ **Parent:** [2A](../2a.md)

For a geodesic [spherical triangle](../../../../../spherical-triangle.md) on a sphere of radius $R$, the [Gauss-Bonnet theorem](../../../../../gauss-bonnet-theorem.md) gives

$$
\boxed{\operatorname{Area}=R^2(\alpha+\beta+\gamma-\pi),}
$$

where $\alpha,\beta,\gamma$ are its interior angles. Indeed, its geodesic sides have zero geodesic curvature, its Gaussian curvature is $R^{-2}$, and its three exterior turning angles sum to $3\pi-(\alpha+\beta+\gamma)$.

Choose a point strictly inside a full-dimensional convex polyhedron and radially project its boundary onto the unit sphere. Triangulate each projected face by diagonals, using only its existing vertices. Convexity ensures that the resulting spherical triangles cover the sphere once, with disjoint interiors. A face with $k$ edges gives $k-2$ triangles, so their number is $T=\sum_{\mathrm{faces}}(k-2)=2E-2F$, since every original edge belongs to two faces.

Sum the spherical excess formula over all triangles. The total area is $4\pi$, and the angles incident to each projected vertex sum to $2\pi$. No additional vertices were introduced by the face triangulations. Hence

$$
4\pi=2\pi V-\pi T=2\pi V-\pi(2E-2F),
\qquad \boxed{F-E+V=2.}
$$

This is the [spherical-triangle proof of the polyhedron Euler formula](../../../../../spherical-triangle-proof-of-the-polyhedron-euler-formula.md).

## ↑ Ancestors (10)

1. [2A](../2a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
