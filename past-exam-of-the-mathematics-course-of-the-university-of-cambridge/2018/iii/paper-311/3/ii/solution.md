<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

By [spherical symmetry](../../../../../../spherical-symmetry.md), rotate a [geodesic](../../../../../../geodesic.md) into the equatorial plane $\theta=\pi/2$. The [geodesic conserved quantities from Killing vectors](../../../../../../geodesic-conserved-quantity-from-a-killing-vector.md) are

$$
E=V\dot t,\qquad L=R^2\dot\varphi,
$$

where the dot denotes a suitable [affine parameter](../../../../../../affine-parameter.md). Normalize the tangent by $g(\dot x,\dot x)=-\epsilon$, with $\epsilon=1$ for timelike proper time, $\epsilon=-1$ for spacelike proper length, and $\epsilon=0$ for null geodesics. Then

$$
-\epsilon=-\frac{E^2}{V}+\frac{\dot r^2}{V}+\frac{L^2}{R^2},\qquad
\dot r^2=E^2-V\left(\epsilon+\frac{L^2}{R^2}\right).
$$

Therefore the [geodesic potential of the magnetic dilaton black hole](../../../../../../geodesic-potential-of-the-magnetic-dilaton-black-hole.md) is

$$
\boxed{\widetilde V(r)=\frac12\left[\left(1-\frac{r_+}{r}\right)\left(\epsilon+\frac{L^2}{r(r-r_-)}\right)-E^2\right].}
$$

Together with the two conserved first integrals, this reduces the radial motion to $\dot r^2/2+\widetilde V=0$. To cover turning points as well, the radial geodesic equation itself gives

$$
\ddot r=-\frac{V'}{2V}(E^2-\dot r^2)+\frac{VL^2R'}{R^3}
=-\frac12\left[V'\left(\epsilon+\frac{L^2}{R^2}\right)-\frac{2VL^2R'}{R^3}\right]=-\widetilde V'.
$$

Thus a constant-radius geodesic must satisfy both $\widetilde V=0$ and $\widetilde V'=0$. The intermediate static-coordinate formulas apply where $V\ne0$; the radial equation extends through a regular horizon in regular coordinates.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 311](../../../paper-311-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
