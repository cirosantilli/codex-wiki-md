<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

**Coordinate surfaces and sketch.** Adding and subtracting the defining relations gives $s=u^2+v^2$ and $x=u^2-v^2$. Since $y^2=s^2-x^2$, we have $y^2=4u^2v^2$. For $u^2=c>0$, eliminate $v^2$ to obtain

$$
x=c-\frac{y^2}{4c}.
$$

This is a [parabolic cylinder](../../../../parabolic-cylinder.md) parallel to the $z$ axis, opening towards negative $x$, with cross-sectional vertex $(c,0)$ and focus at the origin. Similarly, $v^2=d>0$ gives

$$
x=\frac{y^2}{4d}-d,
$$

a [parabolic cylinder](../../../../parabolic-cylinder.md) opening towards positive $x$, with vertex $(-d,0)$ and the same focus. The degenerate $u^2=0$ surface is the half-plane $y=0,x\leq0$; $v^2=0$ gives $y=0,x\geq0$. Constant $w$ gives the horizontal [planes](../../../../plane.md) $z=w$.

Thus the requested cross-sections consist of $x=1-y^2/4$, $x=2-y^2/8$, $x=y^2/4-1$, $x=y^2/8-2$ and the two horizontal half-axes. The [parabolas](../../../../parabola.md) of the two families meet orthogonally.

<a id="1/image-the-requested-parabolic-coordinate-curves-in-the-xy-plane"></a>
![](../../../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2002/paper-1-parabolic-coordinate-net.png)

**[Figure 1](#1/image-the-requested-parabolic-coordinate-curves-in-the-xy-plane). The requested parabolic coordinate curves in the xy plane**. Blue curves have u squared equal to one or two; orange curves have v squared equal to one or two. The thick horizontal rays are the degenerate zero levels. All parabolas share the origin as focus.

**Signed coordinates.** Take $u\geq0$ and choose the sign of $v$ to agree with $y$ away from $y=0$. Then the [Cartesian coordinates](../../../../cartesian-coordinate-system.md) are

$$
\boxed{x=u^2-v^2,\qquad y=2uv,\qquad z=w.}
$$

Every coordinate triple gives exactly one point. For $u>0$, $v$ and $y$ have the same sign. A fixed signed $v\ne0$ selects the upper or lower half of its [parabolic cylinder](../../../../parabolic-cylinder.md); the entire cylinder corresponds to fixed $v^2$. On the cut $u=0$, the two values $v=\pm\sqrt{-x}$ represent the same point of the negative $x$ half-axis. This boundary identification is unavoidable: there $y=0$ even when $v\ne0$, so the sign prescription is understood by approaching from either side of the cut. The interior $u>0$ gives a unique coordinate chart off that half-axis.

**Orthogonality and metric.** Differentiate the [position vector](../../../../position-vector.md):

$$
r_u=(2u,2v,0),\qquad r_v=(-2v,2u,0),\qquad r_w=(0,0,1).
$$

The pairwise [dot products](../../../../dot-product.md) vanish. Their lengths give the [scale factors of orthogonal coordinates](../../../../scale-factors-of-orthogonal-coordinates.md) and hence the [Riemannian metric](../../../../riemannian-metric-split.md):

$$
\boxed{h_u=h_v=2\sqrt{u^2+v^2},\quad h_w=1,\qquad dl^2=4(u^2+v^2)(du^2+dv^2)+dw^2.}
$$

These are [parabolic cylindrical coordinates](../../../../parabolic-cylindrical-coordinates.md). The differential calculation is regular for $u^2+v^2>0$; the $z$ axis is the coordinate singularity where the two planar [tangent vectors](../../../../tangent-vector-split.md) vanish.

**Laplacian.** Put $h=2\sqrt{u^2+v^2}$. The physical components of the [gradient](../../../../gradient.md) of a $w$-independent [scalar field](../../../../scalar-field.md) are $\phi_u/h,\phi_v/h,0$. Applying the [divergence](../../../../divergence.md) formula cancels the two equal [scale factors of orthogonal coordinates](../../../../scale-factors-of-orthogonal-coordinates.md) inside the derivatives:

$$
\nabla^2\phi=\frac1{h^2}\left[\partial_u\left(h\frac{\phi_u}h\right)+\partial_v\left(h\frac{\phi_v}h\right)\right].
$$

Therefore, away from the coordinate singularity,

$$
\boxed{\nabla^2\phi=\frac{\phi_{uu}+\phi_{vv}}{4(u^2+v^2)}.}
$$

## ↑ Ancestors (12)

1. [1](../1.md)
2. [Paper 1](../../paper-1-split.md)
3. [2002](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
