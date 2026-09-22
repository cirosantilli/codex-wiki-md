# Navier slip boundary condition

↑ **Parent:** [Fluid mechanics](fluid-mechanics-split.md)

The [Navier slip boundary condition](navier-slip-boundary-condition.md) allows a [fluid](fluid.md) to slide tangentially past a solid wall while resisting that motion through [wall friction in the Navier slip boundary condition](wall-friction-in-the-navier-slip-boundary-condition.md). For parallel flow past a flat, impermeable wall translating uniformly with tangential [velocity](velocity.md) $U_w$, write the fluid's tangential [velocity](velocity.md) as $u$ and its relative tangential [velocity](velocity.md) as $u_{\mathrm{rel}}=u-U_w$. Then

$$
u_{\mathrm{rel}}=b\partial_nu,\qquad b\ge0,
$$

where $b$ is the [slip length](slip-length.md), also written $\ell_s$. The [unit normal](unit-normal.md) $\mathbf n$ points from the wall into the [fluid](fluid.md), and $\partial_nu=\mathbf n\cdot\nabla u$ is the [normal derivative](normal-derivative.md). The separate [no-penetration boundary condition](no-penetration-boundary-condition.md) requires $(\mathbf u-\mathbf U_w)\cdot\mathbf n=0$: tangential sliding does not allow flow through the wall.

The sign convention matters. In a channel $0<z<H$, the lower wall has inward [unit normal](unit-normal.md) $+\mathbf e_z$ and the upper wall has inward [unit normal](unit-normal.md) $-\mathbf e_z$. If both walls obey the [Navier slip boundary condition](navier-slip-boundary-condition.md), their tangential [velocities](velocity.md) satisfy

$$
u(0)-U_0=b_0u'(0),\qquad
u(H)-U_H=-b_Hu'(H).
$$

Here the prime means the [derivative](derivative.md) with respect to $z$. Using $+b_Hu'(H)$ at the upper wall would reverse the friction law. The examples [Couette flow with a slipping lower wall](couette-flow-with-a-slipping-lower-wall.md) and [planar Poiseuille flow with equal wall slip](planar-poiseuille-flow-with-equal-wall-slip.md) use different upper-wall [boundary conditions](boundary-condition.md).

This flat-wall formula is a local linear model. On a curved wall the [Newtonian fluid stress tensor](newtonian-fluid-stress-tensor.md) must supply the tangential [traction](traction.md); the [normal derivative](normal-derivative.md) alone generally misses curvature terms. The author-written review by Lauga, Brenner and Stone states the full strain-based condition with the [unit normal](unit-normal.md) directed into the liquid. [Lauga, Brenner and Stone, Microfluidics: The No-Slip Boundary Condition (2005), §2.1, equation (2)](https://arxiv.org/pdf/cond-mat/0501557)

The same review credits Navier's 1823 treatise with the linear slip law. Its history is a reminder that the [no-slip boundary condition](no-slip-boundary-condition.md) is an experimentally successful model, whose validity depends on the interface and scale. The history here follows that review rather than a new reading of Navier's original memoir. [Lauga, Brenner and Stone (2005), §2.1: the nineteenth-century boundary-condition debate](https://arxiv.org/pdf/cond-mat/0501557)

**Table of contents**

- [Slip length](slip-length.md)
  - [Couette flow with a slipping lower wall](couette-flow-with-a-slipping-lower-wall.md)
  - [Planar Poiseuille flow with equal wall slip](planar-poiseuille-flow-with-equal-wall-slip.md)
- [Wall friction in the Navier slip boundary condition](wall-friction-in-the-navier-slip-boundary-condition.md)

## ↑ Ancestors (4)

1. [Fluid mechanics](fluid-mechanics-split.md)
2. [Branches of physics](branches-of-physics.md)
3. [Physics](physics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (12)

- [Couette flow with a slipping lower wall](couette-flow-with-a-slipping-lower-wall.md)
- [First-order slip independence of a transverse sheet](first-order-slip-independence-of-a-transverse-sheet.md)
- [Linear basal drag law](linear-basal-drag-law.md)
- [Navier slip boundary condition](navier-slip-boundary-condition.md)
- [Navier-slip Taylor swimming sheet](navier-slip-taylor-swimming-sheet.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-80/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-332/3/solution.md)
- [Planar Poiseuille flow with equal wall slip](planar-poiseuille-flow-with-equal-wall-slip.md)
- [Rarefied gas flow approximations](rarefied-gas-flow-approximations.md)
- [Slip-enhanced swimming speed of a transverse sheet](slip-enhanced-swimming-speed-of-a-transverse-sheet.md)
- [Slip length](slip-length.md)
- [Wall friction in the Navier slip boundary condition](wall-friction-in-the-navier-slip-boundary-condition.md)
