<h1 id="36e/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [incompressibility condition](../../../../../../incompressible-flow.md) turns the left side of the boundary-layer equation into conservative form:

$$
\partial_z(u_z^2)+\frac1r\partial_r(ru_ru_z)=\frac\nu r\partial_r(r\partial_ru_z).
$$

Multiply by $2\pi\rho r$ and integrate from the axis to infinity. Regularity at the axis and decay in the ambient fluid eliminate the radial boundary terms. Thus **the momentum flux is constant**,

$$
\boxed{\frac d{dz}\left(2\pi\rho\int_0^\infty u_z^2r\,dr\right)=0.}
$$

Matching the applied force sets this constant to $F$. Scaling convection against radial viscosity gives $U^2/z\sim\nu U/\delta^2$, while the flux gives $F\sim\rho U^2\delta^2$. Combining them yields

$$
\boxed{U(z)\sim\frac F{\rho\nu z},\qquad \delta(z)\sim\nu\sqrt{\frac\rho F}\,z.}
$$

The slenderness requirement is $\delta/z\sim\nu\sqrt{\rho/F}\ll1$, equivalent to a large force-based Reynolds number $\sqrt{F/\rho}/\nu$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [36E](../../36e.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
