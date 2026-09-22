# Blasius boundary layer

↑ **Parent:** [Boundary layer](boundary-layer.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Blasius_boundary_layer)

A [Blasius boundary layer](blasius-boundary-layer.md) is the [steady flow](steady-flow.md), two-dimensional [laminar flow](laminar-flow.md) along a smooth stationary flat plate with uniform outer [velocity](velocity.md) $U>0$. Let $x>0$ measure distance from its leading edge and $y\geq0$ distance normal to its upper face. For a [Newtonian fluid](newtonian-fluid.md) with constant [mass density](density.md) $\rho$ and [dynamic viscosity](dynamic-viscosity.md) $\mu$, write [kinematic viscosity](kinematic-viscosity.md) $\nu=\mu/\rho$. The [no-slip boundary condition](no-slip-boundary-condition.md) and [impermeability condition](no-penetration-boundary-condition.md) give $u(x,0)=v(x,0)=0$; the streamwise [velocity](velocity.md) approaches $U$ outside the [boundary layer](boundary-layer.md).

<a id="image-computed-laminar-velocity-profiles-and-thickness-measures-along-a-flat-plate"></a>
![](flat-plate-laminar-velocity-profiles.png)

**[Figure 1](#image-computed-laminar-velocity-profiles-and-thickness-measures-along-a-flat-plate). Computed laminar velocity profiles and thickness measures along a flat plate**. The [Blasius equation](blasius-equation.md) supplies all curves. Normal distances are in millimetres and are magnified relative to downstream distances. The dashed [boundary layer thickness](boundary-layer-thickness.md) curve marks $u/U=0.99$, rather than a material interface. The shaded normalized [velocity profile](velocity-profile.md) shows the [displacement thickness](displacement-thickness.md) integrand. Parameters and distances are illustrative model inputs, not experimental measurements.

For example, choose $U=10\,\mathrm{m\,s^{-1}}$ and $\nu=1.5\times10^{-5}\,\mathrm{m^2\,s^{-1}}$. At $x=0.30\,\mathrm m$, the local [Reynolds number](reynolds-number.md) is $\mathrm{Re}_x=Ux/\nu=2.0\times10^5$ and the [boundary layer thickness](boundary-layer-thickness.md) is about $3.29\,\mathrm{mm}$. These illustrative inputs predict a thin [boundary layer](boundary-layer.md); they do not by themselves establish [laminar flow](laminar-flow.md) in an actual [wind tunnel](wind-tunnel.md).

The [boundary-layer scaling](boundary-layer-scaling.md) follows by comparing [advection](advection.md), of size $U^2/x$, with normal viscous transport, of size $\nu U/\delta^2$:

$$
\delta\sim\sqrt{\frac{\nu x}{U}},\qquad \frac{\delta}{x}\sim\mathrm{Re}_x^{-1/2},\qquad \mathrm{Re}_x=\frac{Ux}{\nu}.
$$

Equivalently, the available travel time $x/U$ equals the [viscous diffusion time](viscous-diffusion-time.md) $\delta^2/\nu$ in order of magnitude. Increasing $x$ thickens the [velocity](velocity.md) deficit; increasing $U$ reduces its thickness at a fixed station. This [boundary-layer scaling](boundary-layer-scaling.md) requires $\mathrm{Re}_x\gg1$. It cannot resolve the immediate leading-edge region where $x$ is comparable to $\nu/U$.[Boundary Layer Governing Equations](modules-on-high-reynolds-number-flows/boundary-layer-governing-equations.md)

The [boundary-layer equation](boundary-layer-equation.md) assumes a thin, attached [laminar flow](laminar-flow.md) with streamwise changes over distances much larger than $\delta$, negligible spanwise changes, [incompressible flow](incompressible-flow.md), and constant material properties. For this [Blasius boundary layer](blasius-boundary-layer.md), the outer [pressure gradient](pressure-gradient.md) is zero and wall suction is absent. [Mass conservation](mass-conservation.md) gives $v/U=O(\delta/x)$, but $v u_y$ is still of order $U^2/x$, just like $u u_x$. Thus the [Prandtl boundary-layer equation](prandtl-boundary-layer-equation.md) retains both [advection](advection.md) terms:

$$
u_x+v_y=0,\qquad uu_x+vu_y=\nu u_{yy},\qquad p_y\simeq0.
$$

The discarded streamwise viscous term $\nu u_{xx}$ is smaller than $\nu u_{yy}$ by $O((\delta/x)^2)$. The outer [Euler equations for an inviscid fluid](euler-equations-for-an-inviscid-fluid.md) supply the [pressure](pressure.md); nearly uniform [pressure](pressure.md) across the [boundary layer](boundary-layer.md) does not mean uniform [velocity](velocity.md). [Flow separation](flow-separation.md), substantial wall curvature, [turbulence](turbulence-split.md), or strong changes in outer conditions require reconsidering these hypotheses.

Introduce the [stream function](stream-function.md) and a dimensionless normal coordinate:

$$
\eta=y\sqrt{\frac{U}{\nu x}},\qquad \psi=\sqrt{\nu Ux}\,f(\eta),\qquad u=\psi_y=Uf'(\eta),\qquad v=-\psi_x=\frac12\sqrt{\frac{\nu U}{x}}\,[\eta f'(\eta)-f(\eta)].
$$

Substitution gives the [Blasius equation](blasius-equation.md) $f'''+ff''/2=0$, with $f(0)=f'(0)=0$ and $f'(\infty)=1$. Its numerical [boundary value problem](boundary-value-problem.md) gives $f''(0)\simeq0.332057$. All streamwise [velocity profiles](velocity-profile.md) therefore collapse onto the same $f'(\eta)$ after rescaling $y$ by $\sqrt{\nu x/U}$. The outer normal [velocity](velocity.md) need not vanish: it accounts for the outward displacement accompanying the growing streamwise [velocity](velocity.md) deficit. The MIT [Similarity Solution](modules-on-high-reynolds-number-flows/similarity-solution.md) uses the alternative coordinate $\eta_{\mathrm{MIT}}=\eta/\sqrt2$ and obtains $f_{\mathrm{MIT}}''(0)\simeq0.46960$; its factor of $\sqrt2$ must be converted before comparing [wall shear stress](wall-shear-stress.md).

The historical [Motion of fluids with very little viscosity by L. Prandtl](motion-of-fluids-with-very-little-viscosity-by-l-prandtl.md) already describes a thin transition region that reconciles wall adhesion with the outer [velocity](velocity.md), and a [pressure](pressure.md) distribution imposed by the outer [fluid flow](fluid-flow.md). Its water-channel experiment, described on printed page 8 and in Figure 10, used a paddle wheel, deflectors, and four screens to condition incoming [fluid flow](fluid-flow.md); suspended reflective flakes revealed motion around obstacles. That visual readout supports the importance of near-wall [fluid flow](fluid-flow.md) and [flow separation](flow-separation.md), but it is not a calibrated flat-plate [velocity profile](velocity-profile.md) measurement. A quantitative traverse is described under [flat-plate boundary-layer traverse experiment](flat-plate-boundary-layer-traverse-experiment.md).

**Table of contents**

- [Flat-plate boundary-layer traverse experiment](flat-plate-boundary-layer-traverse-experiment.md)

## ↑ Ancestors (5)

1. [Boundary layer](boundary-layer.md)
2. [Continuum mechanics](continuum-mechanics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Blasius boundary layer](blasius-boundary-layer.md)
- [Boundary layer](boundary-layer.md)
- [Boundary layer thickness](boundary-layer-thickness.md)
- [Displacement thickness](displacement-thickness.md)
- [Flat-plate boundary-layer traverse experiment](flat-plate-boundary-layer-traverse-experiment.md)
- [Momentum thickness](momentum-thickness.md)
- [Skin friction coefficient](skin-friction-coefficient.md)
- [Wall shear stress](wall-shear-stress.md)
