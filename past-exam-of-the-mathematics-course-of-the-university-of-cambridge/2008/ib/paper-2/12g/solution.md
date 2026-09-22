<h1 id="12g/solution">Solution</h1>

↑ **Parent:** [12G](../12g.md)

Work on the unit sphere with geodesic edges. A [spherical lune](../../../../../spherical-lune.md) of angle $\alpha$ has area $\int_0^\alpha\int_0^\pi\sin\theta\,d\theta\,d\varphi=2\alpha$. The three great circles through the sides of a [spherical triangle](../../../../../spherical-triangle.md) partition the sphere into four antipodal pairs of triangles. If the original triangle has area $A$ and the other pair representatives have areas $B,C,D$, then $A+B+C+D=2\pi$. The three lunes at its vertices have areas $A+B,A+C,A+D$, so

$$
2(\alpha+\beta+\gamma)=3A+B+C+D=2A+2\pi.
$$

This proves the [spherical excess formula](../../../../../spherical-excess-formula.md) $\boxed{A=\alpha+\beta+\gamma-\pi}$. Triangulate a convex spherical $k$-gon from one vertex into $k-2$ triangles; summing areas and vertex angles gives

$$
\boxed{A_k=\sum_{j=1}^k\alpha_j-(k-2)\pi.}
$$

For a decomposition of the whole sphere, angles around every vertex sum to $2\pi$ and each edge belongs to two faces. Summing the polygon area formula over all faces therefore gives

$$
4\pi=2\pi V-\pi(2E-2F),\qquad
\boxed{F-E+V=2}.
$$

Now $F=m+n+p$, $2E=4m+5n+6p$, and $3V=2E$, since three edges meet at each vertex. Substituting into Euler's formula yields $2m+n=12$. Nonnegative integer solutions therefore give at most seven pairs:

$$
\boxed{(m,n)=(0,12),(1,10),(2,8),(3,6),(4,4),(5,2),(6,0).}
$$

At least three distinct pairs are realized: a [dodecahedron](../../../../../dodecahedron.md) gives $(0,12)$, a [pentagonal prism](../../../../../pentagonal-prism.md) gives $(5,2)$, and a [cube](../../../../../cube.md) gives $(6,0)$. Center each convex polyhedron around an interior origin and radially project its faces onto the sphere; edges become great-circle arcs and the resulting spherical faces are convex, preserving the incidence counts. This supplies the required actual decompositions.

## ↑ Ancestors (10)

1. [12G](../12g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
