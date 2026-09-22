<h1 id="20/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take a face on the flat base and let $x,y$ be its positive half-widths, with height $z>0$. The upper vertices meet the spherical boundary at $x^2+y^2+z^2=a^2$, and the [rectangular parallelepiped](../../../../../rectangular-parallelepiped.md) has [volume](../../../../../volume.md) $V=4xyz$. A [Lagrange multiplier](../../../../../lagrange-multiplier.md) gives

$$
4yz=2\lambda x,\qquad4xz=2\lambda y,\qquad4xy=2\lambda z.
$$

Multiplication by $x,y,z$ respectively shows $x^2=y^2=z^2$. Positivity and the constraint give $x=y=z=a/\sqrt3$. Therefore

$$
\boxed{V_{\max}=\frac{4a^3}{3\sqrt3},\qquad
\text{edge lengths }\frac{2a}{\sqrt3},\ \frac{2a}{\sqrt3},\ \frac a{\sqrt3}.}
$$

Boundary choices with a zero dimension give zero [volume](../../../../../volume.md), so this is the maximum in this configuration.

The [maximum-volume cuboid in a hemisphere](../../../../../maximum-volume-cuboid-in-a-hemisphere.md) also has a bound covering arbitrary orientations. Let $u_i$ be any box's half-edge lengths, $v_i$ its [centre](../../../../../center-geometry.md) coordinates in its orthonormal edge [basis](../../../../../basis.md), and $n_i$ the vertical unit-vector coordinates. Remaining above the base [plane](../../../../../plane.md) requires $\sum n_iv_i\geq\sum|n_i|u_i$, so $|v_j|\geq u_j$ for at least one index. Its farthest vertex obeys

$$
a^2\geq R_{\max}^2=\sum u_i^2+\sum v_i^2+2\sum u_i|v_i|
\geq\sum_{i\ne j}u_i^2+4u_j^2,
$$

where containment supplies the first inequality. The [arithmetic-geometric mean inequality](../../../../../arithmetic-geometric-mean-inequality.md) applied to the three terms $u_i^2$ for $i\ne j$ and $4u_j^2$ yields $2u_1u_2u_3\leq a^3/(3\sqrt3)$. Thus its full [volume](../../../../../volume.md) $8u_1u_2u_3$ cannot exceed the value attained above; tilting cannot improve it. Boundary contact is allowed for the maximum; strict containment would give the same supremum.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [20](../../20.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
