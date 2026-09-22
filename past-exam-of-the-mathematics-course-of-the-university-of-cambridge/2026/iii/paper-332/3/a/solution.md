<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [shallow-ice approximation](../../../../../../shallow-ice-approximation.md) makes the pressure [hydrostatic pressure](../../../../../../hydrostatic-pressure.md),

$$
p=\rho g(h-z),
\qquad
p_x=\rho g h_x.
$$

Horizontal [Stokes flow](../../../../../../stokes-flow-split.md) balance and the [stress-free boundary condition](../../../../../../stress-free-boundary-condition.md) at $z=h$ give

$$
\mu u_{zz}=\rho g h_x,
\qquad
u_z(h)=0,
$$

so

$$
u_z=\frac{\rho g}{\mu}h_x(z-h).
$$

The basal shear stress and the stated [basal sliding](../../../../../../basal-sliding.md) law are therefore

$$
\boxed{\tau_b=\mu u_z(0)=-\rho ghh_x},
\qquad
\boxed{u_b=-\beta h_x}.
$$

Integrating once more and imposing $u(0)=u_b$ yields

$$
\boxed{
u(x,z,t)=-\beta h_x
+\frac{\rho g}{2\mu}h_x(z^2-2hz)}.
$$

For the right half of an [ice cap](../../../../../../ice-cap.md), $h_x<0$, so both basal sliding and internal deformation carry ice away from the [ice divide](../../../../../../ice-divide.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 332](../../../paper-332-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
