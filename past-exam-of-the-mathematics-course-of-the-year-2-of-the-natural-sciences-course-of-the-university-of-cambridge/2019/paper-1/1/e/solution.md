<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The ellipse bounding the surface is $u=1$. With the upward normal, its positively oriented boundary is traversed by increasing $v$ from zero to $2\pi$:

$$
\mathbf r(v)=(a\cosh1\cos v,a\sinh1\sin v,c),\qquad d\mathbf r=(-a\cosh1\sin v,a\sinh1\cos v,0)dv.
$$

The given components are Cartesian components, so their ordinary [dot product](../../../../../dot-product.md) with this tangent is

$$
\mathbf F\cdot d\mathbf r=-2a\sinh1\cosh1(\sin^2v+\cos^2v)dv.
$$

Therefore [Stokes theorem](../../../../../stokes-theorem.md) gives

$$
\boxed{\int_S(\nabla\times\mathbf F)\cdot d\mathbf S=-4\pi a\sinh1\cosh1=-2\pi a\sinh2.}
$$

A direct check uses $F_x=2y/a$ and $F_y=-2x/a$, hence $(\nabla\times\mathbf F)_z=-4/a$, and multiplies by the ellipse area $\pi a^2\sinh1\cosh1$. The third component cannot affect either calculation because the surface and its boundary lie at fixed $z$. Equivalently one may apply Stokes to the smooth planar field $(2y/a,-2x/a,0)$, avoiding any need to differentiate the elliptic-coordinate expression for the third component at its foci.

## ↑ Ancestors (13)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
