<h1 id="4b/solution">Solution</h1>

↑ **Parent:** [4B](../4b.md)

For a [spherical triangle](../../../../../spherical-triangle.md) on a sphere of radius $R$, bounded by shorter [great circle](../../../../../great-circle.md) arcs and with interior angles $\alpha,\beta,\gamma$, the [spherical excess formula](../../../../../spherical-excess-formula.md), the triangular form of the [Gauss-Bonnet theorem](../../../../../gauss-bonnet-theorem.md), is

$$
\boxed{\operatorname{area}=R^2(\alpha+\beta+\gamma-\pi).}
$$

Here is an area proof. On the unit sphere, a [spherical lune](../../../../../spherical-lune.md) of angle $\alpha$ has area $2\alpha$: rotating around its vertices shows it occupies a fraction $\alpha/(2\pi)$ of the sphere when one uses the full angular width, or directly integrates $\int_0^\alpha\int_0^\pi\sin\theta\,d\theta\,d\varphi$. The three side great circles of the triangle divide the sphere into eight regions, including the triangle $T$ and its antipodal triangle $-T$. Choose, at each vertex, the lune containing $T$, and also its antipodal lune. Each of $T$ and $-T$ is covered three times by these six lunes; each other region is covered once. Thus, with $A$ the area of $T$,

$$
4(\alpha+\beta+\gamma)=4\pi+4A.
$$

This proves $A=\alpha+\beta+\gamma-\pi$; scaling lengths by $R$ scales area by $R^2$.

Radially project each face of the regular [dodecahedron](../../../../../dodecahedron.md) from its centre onto the unit sphere. Each edge and the origin lie in a plane, so its image is a shorter [great circle](../../../../../great-circle.md) arc. The twelve faces give congruent [convex regular spherical polygons](../../../../../convex-regular-spherical-polygon.md) partitioning the sphere. At each projected vertex three congruent face angles fill the tangent plane. Hence each spherical pentagon has angle $2\pi/3$ at each of its five vertices. Splitting a pentagon into three [spherical triangles](../../../../../spherical-triangle.md) and summing the [spherical excess formula](../../../../../spherical-excess-formula.md) gives

$$
\operatorname{area}=5\frac{2\pi}{3}-3\pi=\boxed{\frac\pi3},\qquad
\boxed{\text{each angle}=\frac{2\pi}{3}}.
$$

This also agrees with $4\pi/12$, as required by the spherical partition.

## ↑ Ancestors (10)

1. [4B](../4b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
