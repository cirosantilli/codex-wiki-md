# Wall friction in the Navier slip boundary condition

↑ **Parent:** [Navier slip boundary condition](navier-slip-boundary-condition.md)

For a [Newtonian fluid](newtonian-fluid.md) and a flat wall with $0<b<\infty$, the [Navier slip boundary condition](navier-slip-boundary-condition.md) is equivalent to a tangential wall-on-fluid [traction](traction.md)

$$
t_{w,t}=-\frac{\mu}{b}u_{\mathrm{rel}}.
$$

The sign expresses resisting [friction](friction.md): $\partial_nu$ uses the inward [unit normal](unit-normal.md), whereas the wall-on-fluid [traction](traction.md) uses the outward [unit normal](unit-normal.md) of the fluid domain. The irreversible loss of mechanical [energy](energy.md) per unit wall [area](surface-area.md) and time is

$$
\mathcal D_w=-t_{w,t}u_{\mathrm{rel}}
=\frac{\mu}{b}u_{\mathrm{rel}}^2\ge0,
\qquad [\mathcal D_w]=\mathrm{W\,m^{-2}}.
$$

For two tangential directions replace $u_{\mathrm{rel}}^2$ by the squared [Euclidean norm](euclidean-norm.md) of relative tangential [velocity](velocity.md). At a moving wall this relative-[velocity](velocity.md) loss must be distinguished from the [power](power.md) supplied by the wall's motion. Bulk [viscous dissipation](viscous-dissipation.md) also remains present. A finite [slip length](slip-length.md) models reduced interfacial resistance, without declaring every boundary ideal or removing [dynamic viscosity](dynamic-viscosity.md).

The limiting loss depends on how the flow is driven. In [Couette flow with a slipping lower wall](couette-flow-with-a-slipping-lower-wall.md),

$$
\mathcal D_w=\frac{\mu U^2b}{(H+b)^2}.
$$

It tends to zero for both $b\to0$ and $b\to\infty$ at fixed $H$ and $U$. At $b=0$ impose the [no-slip boundary condition](no-slip-boundary-condition.md) directly, rather than dividing by zero. In [planar Poiseuille flow with equal wall slip](planar-poiseuille-flow-with-equal-wall-slip.md) at fixed $G$, each wall instead dissipates $G^2bH^2/(4\mu)$, which grows with $b$ because relative [velocity](velocity.md) grows. The bulk loss per unit width is $G^2H^3/(12\mu)$; adding both wall losses gives $Gq$, the [pressure](pressure.md) work per unit channel length and width. This [energy](energy.md) balance shows why small friction coefficients do not guarantee small losses under every driving constraint.

## ↑ Ancestors (5)

1. [Navier slip boundary condition](navier-slip-boundary-condition.md)
2. [Fluid mechanics](fluid-mechanics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Navier slip boundary condition](navier-slip-boundary-condition.md)
