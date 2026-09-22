<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For $a>0$, the positive constant-$u$ surfaces in [elliptic cylindrical coordinates](../../../../elliptic-cylindrical-coordinates.md) satisfy

$$
\frac{x^2}{a^2\cosh^2u}+\frac{y^2}{a^2\sinh^2u}=1.
$$

They are confocal [elliptic cylinders](../../../../elliptic-cylinder.md) with focal lines $x=\pm a,y=0$. For a generic fixed $v$, eliminating $u$ gives

$$
\frac{x^2}{a^2\cos^2v}-\frac{y^2}{a^2\sin^2v}=1.
$$

Because $u\geq0$, a fixed $v$ selects the half-branch with the signs of $x$ and $y$ fixed by $\cos v$ and $\sin v$. These are [hyperbolic cylinders](../../../../hyperbolic-cylinder.md). The degenerate $u=0$ surface is $y=0$, $|x|\leq a$, extended in $z$. At $v=0,\pi$ the cross-sections are the two exterior horizontal rays; at $v=\pi/2,3\pi/2$ they are vertical half-axes.

<a id="1/image-confocal-elliptic-and-hyperbolic-coordinate-curves"></a>
![](../../../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2003/paper-1-elliptic-coordinate-net.png)

**[Figure 1](#1/image-confocal-elliptic-and-hyperbolic-coordinate-curves). Confocal elliptic and hyperbolic coordinate curves**. Original cross-section with focal points marked. Ellipses are constant-u curves and the hyperbola half-branches are constant-v curves; extruding in z gives their coordinate surfaces.

Differentiate the position [vector](../../../../vector.md) to get the coordinate [tangent vectors](../../../../tangent-vector-split.md)

$$
r_u=(a\sinh u\cos v,a\cosh u\sin v,0),\quad r_v=(-a\cosh u\sin v,a\sinh u\cos v,0),\quad r_z=(0,0,1).
$$

Their pairwise [dot products](../../../../dot-product.md) vanish. Their squared lengths are $a^2(\sinh^2u+\sin^2v)$, $a^2(\sinh^2u+\sin^2v)$ and one. This proves [orthogonality](../../../../orthogonal-vectors.md) and gives the [scale factors of orthogonal coordinates](../../../../scale-factors-of-orthogonal-coordinates.md):

$$
\boxed{h_u=h_v=h=a\sqrt{\sinh^2u+\sin^2v},\qquad h_z=1.}
$$

The [Riemannian metric](../../../../riemannian-metric-split.md) is $ds^2=h^2(du^2+dv^2)+dz^2$. Away from the focal lines, divide the coordinate [tangent vectors](../../../../tangent-vector-split.md) by their lengths to obtain the local orthonormal [unit vectors](../../../../unit-vector.md) $e_u,e_v,e_z$. For physical [vector field](../../../../vector-field.md) components $A_u,A_v,A_z$, the formulas for [vector calculus in elliptic cylindrical coordinates](../../../../vector-calculus-in-elliptic-cylindrical-coordinates.md) are

$$
\boxed{\nabla\cdot A=\frac{\partial_u(hA_u)+\partial_v(hA_v)+\partial_z(h^2A_z)}{h^2},}
$$



$$
\boxed{\nabla\times A=\frac{\partial_vA_z-\partial_z(hA_v)}h e_u+\frac{\partial_z(hA_u)-\partial_uA_z}h e_v+\frac{\partial_u(hA_v)-\partial_v(hA_u)}{h^2}e_z.}
$$

The [gradient](../../../../gradient.md) of a [scalar](../../../../scalar.md) [function](../../../../function-split.md) has components $(\phi_u/h,\phi_v/h,\phi_z)$. Apply the [divergence](../../../../divergence.md) formula to this [gradient](../../../../gradient.md); [Laplace's equation](../../../../laplace-equation.md) becomes

$$
\boxed{\frac{\phi_{uu}+\phi_{vv}}{a^2(\sinh^2u+\sin^2v)}+\phi_{zz}=0.}
$$

The formulas apply where $h>0$; the focal lines require a limit or another coordinate chart.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [Paper 1](../../paper-1-split.md)
3. [2003](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
