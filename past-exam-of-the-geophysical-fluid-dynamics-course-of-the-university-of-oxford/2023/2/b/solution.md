<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [quasi-geostrophic potential-vorticity equation](../../../../quasi-geostrophic-potential-vorticity-equation.md) is the leading balanced form of [potential-vorticity conservation](../../../../potential-vorticity-conservation.md) for an inviscid rotating fluid with [stable density stratification](../../../../stable-density-stratification.md), small [Rossby number](../../../../rossby-number.md) and an [adiabatic process](../../../../adiabatic-process.md) for each [fluid element](../../../../fluid-element.md). Its parent conservation law is [Ertel potential vorticity](../../../../ertel-potential-vorticity.md) conservation. Horizontal [geostrophic balance](../../../../geostrophic-balance.md), vertical [hydrostatic balance](../../../../hydrostatic-balance.md), and the [beta-plane approximation](../../../../beta-plane.md) reduce it to advection of one scalar by the leading horizontal [geostrophic flow](../../../../geostrophic-flow.md).

One can see its origin by combining the vertical [vorticity equation](../../../../vorticity-equation.md) with the thermal equation. Set $D_g=\partial_t+\mathbf u_g\cdot\nabla_h$, $\mathbf u_g=(-\psi_y,\psi_x)$, and $\zeta_g=\nabla_h^2\psi$. The [quasi-geostrophic approximation](../../../../quasi-geostrophic-approximation.md) gives

$$
D_g(\zeta_g+f_0+\beta y)=f_0w_z,
\qquad
D_gb+N^2w=0,\qquad b=f_0\psi_z.
$$

Here $b$ is the [buoyancy perturbation](../../../../buoyancy-perturbation.md) relative to the reference [stable density stratification](../../../../stable-density-stratification.md), $N=N(z)$ its [buoyancy frequency](../../../../buoyancy-frequency.md), and $w$ the small vertical [velocity](../../../../velocity.md). The stretching of absolute [vorticity](../../../../vorticity-split.md) in the first equation is offset by the change of [stratification](../../../../density-stratification.md) represented by the second. More precisely,

$$
D_g\partial_z\left(\frac{f_0b}{N^2}\right)
=\partial_z\left(\frac{f_0D_gb}{N^2}\right)
-\frac{f_0}{N^2}(\partial_z\mathbf u_g)\cdot\nabla_hb
=-f_0w_z.
$$

The last [dot product](../../../../dot-product.md) is zero because [thermal-wind balance](../../../../thermal-wind.md) makes $\partial_z\mathbf u_g$ perpendicular to $\nabla_hb$. Adding therefore yields

$$
\boxed{D_gq=0,\qquad
q=\underbrace{\nabla_h^2\psi}_{\text{relative vorticity}}
+\underbrace{f_0+\beta y}_{\text{planetary vorticity}}
+\underbrace{\partial_z\left(\frac{f_0^2}{N^2}\psi_z\right)}_{\text{stratification/stretching contribution}}.}
$$

The constant $f_0$ has no effect on the tendency, but its inclusion makes the connection with absolute [vorticity](../../../../vorticity-split.md) clear. Vertical [advection](../../../../advection.md) of $q$ is beyond the retained order; the vertical [velocity](../../../../velocity.md) has already supplied the stretching and thermodynamic terms.

For a simple balanced weather forecast, the essential cycle is **diagnose, advect, invert**:


- Use observed [pressure](../../../../pressure-split.md) or [geopotential](../../../../geopotential.md) and [temperature](../../../../temperature-split.md) to construct a balanced initial [quasi-geostrophic streamfunction](../../../../quasi-geostrophic-streamfunction.md), its interior [potential vorticity](../../../../potential-vorticity.md), and the upper and lower boundary [buoyancy](../../../../buoyancy.md).
- Evolve $q$ with $q_t=-\mathbf u_g\cdot\nabla_hq$ for a small time step. For flat rigid boundaries, also evolve their thermal data with $D_gb=0$ there. Appropriate lateral [boundary conditions](../../../../boundary-condition.md) and any known large-scale circulation must accompany these fields.
- Recover the new [streamfunction](../../../../stream-function.md) by [stratified quasi-geostrophic inversion](../../../../stratified-quasi-geostrophic-inversion.md):


$$
\left[\nabla_h^2+\partial_z\left(\frac{f_0^2}{N^2}\partial_z\right)\right]\psi
=q-f_0-\beta y.
$$

This is an [elliptic boundary value problem](../../../../elliptic-boundary-value-problem-split.md), not a local algebraic diagnosis. Its solution supplies the next [geostrophic flow](../../../../geostrophic-flow.md) and, through $b=f_0\psi_z$, the next thermal field. Repeat the cycle to move the balanced weather systems forward.

Interior [potential vorticity](../../../../potential-vorticity.md) alone is insufficient: boundary thermal anomalies can induce flow even with zero interior anomaly, as in the [Eady model](../../../../eady-model.md). The method filters fast [inertia-gravity waves](../../../../inertia-gravity-wave.md) and is useful for large-scale extratropical weather, while tropical dynamics, [convection](../../../../convection-split.md), moisture, friction and diabatic heating require additional physics. If vertical motion is wanted, the [quasi-geostrophic omega equation](../../../../quasi-geostrophic-omega-equation.md) supplies a further diagnostic calculation.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the geophysical fluid dynamics course of the University of Oxford](../../../split.md)
5. [Geophysical fluid dynamics course of the University of Oxford](../../../../geophysical-fluid-dynamics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
