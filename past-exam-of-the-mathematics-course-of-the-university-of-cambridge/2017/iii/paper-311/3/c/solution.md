<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the zero-angular-momentum curves, the fiber term in the induced [metric tensor](../../../../../../metric-tensor.md) vanishes along the tangent, leaving

$$
0=-\frac f h\dot t^2+\frac{\dot r^2}{f}
$$

for a [null geodesic](../../../../../../null-geodesic.md). In the exterior, a future [geodesic](../../../../../../geodesic.md) has positive conserved [energy](../../../../../../energy.md) $E=(f/h)\dot t$. Its equations are

$$
\dot r=\pm E\sqrt h,\qquad \dot t=\frac{Eh}{f},\qquad
\frac{dt}{dr}=\pm\frac{\sqrt h}{f}.
$$

Define the [tortoise coordinate](../../../../../../tortoise-coordinate.md), separately on intervals bounded by horizon radii, by

$$
\boxed{r_*(r)=\int^r\frac{\sqrt{h(s)}}{f(s)}\,ds.}
$$

For an outgoing curve $\dot r=+E\sqrt h$,

$$
\frac d{d\lambda}(t-r_*)=\dot t-r_*'\dot r=0;
$$

for an ingoing curve $\dot r=-E\sqrt h$, $d(t+r_*)/d\lambda=0$. Thus $u=t-r_*$ and $v=t+r_*$ are the respective constant labels. The [derivative](../../../../../../derivative.md) $\sqrt h/f$, with its sign, is required for continuation; taking $\sqrt h/|f|$ would give the wrong labels between the horizons.

For a nonextremal horizon $r=r_H$, the [tortoise coordinate](../../../../../../tortoise-coordinate.md) has leading behavior

$$
r_*\sim\frac{\sqrt{h(r_H)}}{f'(r_H)}\log|r-r_H|.
$$

At the double root of the [extremal black hole](../../../../../../extremal-black-hole.md) it instead has a pole. These singularities are coordinate effects at a regular [Killing horizon](../../../../../../killing-horizon.md); they are not the [curvature singularity](../../../../../../curvature-singularity.md) at $r=0$. To cross the future horizon, the ingoing coordinates

$$
v=t+r_*,\qquad \psi_+=\psi+\int^r\frac{\Omega(s)\sqrt{h(s)}}{f(s)}\,ds
$$

give the regular induced [metric tensor](../../../../../../metric-tensor.md)

$$
ds_3^2=-\frac f h\,dv^2+\frac2{\sqrt h}\,dv\,dr
+r^2h(d\psi_+-\Omega\,dv)^2.
$$

This also fixes the future branch used in the causal argument below.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 311](../../../paper-311-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
