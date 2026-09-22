<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take $x$ along a horizontal gap and $s$ perpendicular to its plates, with $0<s<b$. Assume a [Newtonian fluid](../../../../newtonian-fluid.md), stationary plates, a [steady flow](../../../../steady-flow.md), a [laminar flow](../../../../laminar-flow.md) and a [fully developed flow](../../../../fully-developed-flow.md) away from the entrances and side edges. The [no-slip boundary condition](../../../../no-slip-boundary-condition.md) holds on both plates. Any transverse [gravity](../../../../gravity.md) is absorbed in the [hydrostatic pressure](../../../../hydrostatic-pressure.md); there is no imposed transverse through-flow. Translational symmetry and the [no-penetration boundary condition](../../../../no-penetration-boundary-condition.md) then give $\mathbf u=(u(s),0,0)$. The [Navier-Stokes equation](../../../../navier-stokes-equation.md) reduces to

$$
0=-\frac{dp}{dx}+\eta\frac{d^2u}{ds^2},\qquad
\frac{dp}{dx}=-\frac{\Delta p}{L},\qquad u(0)=u(b)=0.
$$

Twice integrating gives the [plane Poiseuille flow](../../../../plane-poiseuille-flow.md):

$$
\boxed{u_x(s)=\frac{\Delta p}{2\eta L}s(b-s),\qquad u_s=u_{\mathrm{span}}=0.}
$$

The [volumetric flow rate](../../../../volumetric-flow-rate.md) through one gap is

$$
Q_{\mathrm{gap}}=w\int_0^b u_x(s)\,ds
=\frac{wb^3\Delta p}{12\eta L}.
$$

There are $n-1$ internal gaps. Their total cross-sectional area is $(n-1)wb$, because the plate thickness is negligible, so the [Darcy velocity](../../../../darcy-velocity.md) is

$$
\boxed{q=\frac{(n-1)Q_{\mathrm{gap}}}{(n-1)wb}
=\frac{b^2}{12\eta}\frac{\Delta p}{L},\qquad \Pi_0=\frac{b^2}{12}.}
$$

Thus the [permeability of a porous medium](../../../../permeability-of-a-porous-medium.md) has the dimensions of squared [length](../../../../length.md). If finite plate thickness were included, the [Darcy velocity](../../../../darcy-velocity.md) averaged over the whole manifold would also contain its [porosity](../../../../porosity.md).

Both the local [acceleration](../../../../acceleration.md) and the [convective acceleration](../../../../convective-acceleration.md) vanish: $\partial_t\mathbf u=0$ and $(\mathbf u\cdot\nabla)\mathbf u=u_x\partial_x\mathbf u=0$. The dominant balance is therefore between the [pressure gradient](../../../../pressure-gradient.md) and [viscous stress](../../../../viscous-stress-tensor.md), with no [inertia](../../../../inertia.md) contribution in this fully developed solution. This exact cancellation does not guarantee that arbitrary large-[Reynolds number](../../../../reynolds-number.md) realizations remain [laminar flows](../../../../laminar-flow.md); entrances, disturbances and [turbulence](../../../../turbulence-split.md) can invalidate the assumptions.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the fluids course of the University of Oxford](../../../split.md)
5. [Fluids course of the University of Oxford](../../../../fluids-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
