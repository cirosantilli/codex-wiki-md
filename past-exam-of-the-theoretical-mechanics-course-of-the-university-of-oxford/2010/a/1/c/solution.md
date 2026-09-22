<h1 id="a/1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a steady unidirectional field $\mathbf u=w\mathbf k$, [incompressibility](../../../../../incompressible-flow.md) gives $\partial_z w=0$. Thus $w=w(x,y)$ and the convective acceleration vanishes. The transverse momentum equations give $p_x=p_y=0$, so $p=p(z)$. The axial equation is

$$
\mu\Delta_\perp w=p'(z).
$$

Its left side is independent of $z$ and its right side independent of $x,y$, so both equal a constant $G$. No slip against the translating wall gives $w=U$ on the boundary. Thus the asserted Poisson problem follows.

For the circular pipe, the axisymmetric solution is

$$
\boxed{w(r)=U+\frac G{4\mu}(r^2-R^2).}
$$

It satisfies the boundary value and $\Delta_\perp r^2=4$. Integrating over the cross-section gives

$$
Q=2\pi\int_0^Rw(r)r\,dr=\pi R^2U-\frac{\pi R^4G}{8\mu}.
$$

Therefore the laboratory-frame [volume flux](../../../../../volumetric-flow-rate.md) vanishes precisely when

$$
\boxed{U=\frac{R^2}{8\mu}\frac{dp}{dz}.}
$$

For a [pressure](../../../../../pressure-split.md) decrease in the positive axial direction, this requires upstream wall translation.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the theoretical mechanics course of the University of Oxford](../../../../split.md)
6. [Theoretical mechanics course of the University of Oxford](../../../../../theoretical-mechanics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
