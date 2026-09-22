<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $H$ be the typical thickness, $\ell_r$ the radial variation [length](../../../../length.md), $U$ the horizontal [speed](../../../../speed.md), and $W$ the vertical [speed](../../../../speed.md). For a thin smooth profile, $\varepsilon=H/\ell_r\ll1$. The axisymmetric [continuity equation](../../../../continuity-equation.md) is

$$
\frac1r\partial_r(rv_r)+\partial_zv_z=0.
$$

Away from singular boundary regions, balancing its terms gives $U/\ell_r\sim W/H$, hence $\boxed{W/U\sim\varepsilon\ll1}$. Near $r=0$, regularity gives $v_r=O(r)$ and the same conclusion follows without a divergent $v_r/r$ term.

Vertical viscous [derivatives](../../../../derivative.md) dominate horizontal ones by $\varepsilon^{-2}$. The ratio of [convective acceleration](../../../../convective-acceleration.md) to vertical viscous [acceleration](../../../../acceleration.md) is

$$
\frac{U^2/\ell_r}{\nu U/H^2}=\frac{UH^2}{\nu\ell_r}.
$$

For thickness-evolution time $T$, the local inertial ratio is $H^2/(\nu T)$. When both ratios are small, [lubrication theory](../../../../lubrication-theory.md) reduces the [Navier-Stokes equation](../../../../navier-stokes-equation.md) to

$$
\boxed{0\approx\mu\partial_z^2\mathbf v-\nabla p-\rho g\widehat{\mathbf z}.}
$$

Thinness must therefore accompany a slow enough motion; it is not a justification for dropping arbitrarily rapid imposed [acceleration](../../../../acceleration.md). The small vertical [velocity](../../../../velocity.md) also makes the leading vertical balance [hydrostatic balance](../../../../hydrostatic-balance.md), $p_z=-\rho g$. The neglected normal viscous [stress](../../../../stress.md) at the interface is smaller than the characteristic lubrication [pressure](../../../../pressure-split.md) by order $\varepsilon^2$.

Use the source's [curvature](../../../../curvature.md) sign: $p_{\mathrm{air}}-p_{\mathrm{liquid}}=-\gamma\kappa$. The [Young–Laplace equation](../../../../young-laplace-equation.md) and atmospheric [pressure](../../../../pressure-split.md) $p_0$ thus give $p(r,h,t)=p_0+\gamma\kappa$. Integrating the [hydrostatic balance](../../../../hydrostatic-balance.md) yields

$$
\boxed{p(r,z,t)=p_0+\gamma\kappa(r,t)+\rho g[h(r,t)-z].}
$$

Consequently $p_r=\gamma\kappa_r+\rho gh_r$, independent of $z$ at this order. The radial [Stokes equation](../../../../stokes-equation.md) and [boundary conditions](../../../../boundary-condition.md) are

$$
\mu\partial_z^2v_r=p_r,\qquad
v_r(r,0,t)=0,\qquad \partial_zv_r(r,h,t)=0.
$$

The first is the [no-slip boundary condition](../../../../no-slip-boundary-condition.md); the second is the leading [stress-free boundary condition](../../../../stress-free-boundary-condition.md), since the atmosphere has negligible [dynamic viscosity](../../../../dynamic-viscosity-split.md) and the [surface tension](../../../../surface-tension-split.md) is constant. Integrating twice gives

$$
\boxed{\mathbf v_h\approx
\left(\rho gh_r+\gamma\kappa_r\right)\frac{z(z-2h)}{2\mu}\widehat{\mathbf r}.}
$$

This is the horizontal [velocity](../../../../velocity.md) only. A smaller vertical [velocity](../../../../velocity.md) is generally required by the [continuity equation](../../../../continuity-equation.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the fluids course of the University of Oxford](../../../split.md)
5. [Fluids course of the University of Oxford](../../../../fluids-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
