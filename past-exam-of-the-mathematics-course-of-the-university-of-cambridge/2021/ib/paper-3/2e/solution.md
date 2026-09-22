<h1 id="2e/solution">Solution</h1>

↑ **Parent:** [2E](../2e.md)

For a [geodesic triangle](../../../../../geodesic-triangle.md) with interior angles $\alpha,\beta,\gamma$, the local [Gauss-Bonnet theorem](../../../../../gauss-bonnet-theorem.md) is

$$
\boxed{\int_TK\,dA=\alpha+\beta+\gamma-\pi},
$$

because its geodesic sides have zero [geodesic curvature](../../../../../geodesic-curvature.md).

Triangulate a closed oriented surface into $F$ geodesic triangles, with $E$ edges and $V$ vertices. Summing the local formula, the angles around each vertex total $2\pi$, so

$$
\int_SK\,dA=2\pi V-\pi F.
$$

Since every triangular face has three edges and every edge belongs to two faces, $3F=2E$. Hence

$$
\int_SK\,dA=2\pi(V-E+F)
=\boxed{2\pi\chi(S)},
$$

which is the global Gauss-Bonnet theorem.

For the sphere $S_r$, the unit normal is $N(p)=p/r$. Its [shape operator](../../../../../shape-operator.md) is, up to the conventional sign, $(1/r)I$ on each tangent plane. Both [principal curvatures](../../../../../principal-curvature.md) therefore have magnitude $1/r$, and the [Gaussian curvature](../../../../../gaussian-curvature.md) is

$$
\boxed{K=\frac1{r^2}}.
$$

An octant has one eighth of the sphere's area:

$$
\operatorname{area}(T)=\frac18(4\pi r^2)=\frac{\pi r^2}{2}.
$$

Thus $\int_TK\,dA=\pi/2$. Its three great-circle sides meet at three right angles, so

$$
\alpha+\beta+\gamma-\pi
=3\frac\pi2-\pi=\frac\pi2.
$$

The two sides of the local Gauss-Bonnet formula agree directly.

## ↑ Ancestors (10)

1. [2E](../2e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
