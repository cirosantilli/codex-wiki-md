<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $b$ denote [buoyancy](../../../../buoyancy.md) in a stably stratified [Boussinesq approximation](../../../../boussinesq-approximation.md). [Geostrophic balance](../../../../geostrophic-balance.md) and [hydrostatic balance](../../../../hydrostatic-balance.md) imply the [thermal wind](../../../../thermal-wind.md) relation $f_0U_z=-\bar b_y$. Consequently the specified vertical shear requires

$$
\boxed{\bar b_y=-f_0\Lambda,\qquad \bar b_z=N^2>0}.
$$

For northern-hemisphere $f_0>0$ and $\Lambda>0$, the mean [potential temperature](../../../../potential-temperature.md) decreases northward and increases upward: $\bar\Theta_y=-(\Theta_0/g)f_0\Lambda$, $\bar\Theta_z=(\Theta_0/g)N^2$. The corresponding mean isentropes slope upward toward the north, with $dz/dy=f_0\Lambda/N^2$. Stable potential-temperature stratification does not require the actual [temperature](../../../../temperature-split.md) to increase upward; the dry adiabatic lapse also enters that comparison.

In the [rigid-lid constant-shear baroclinic model](../../../../rigid-lid-constant-shear-baroclinic-model.md), perturbation [quasi-geostrophic potential vorticity](../../../../three-dimensional-quasi-geostrophic-potential-vorticity.md) is

$$
q'=\nabla_h^2\psi'+\frac{f_0^2}{N^2}\psi'_{zz}.
$$

The mean interior potential-vorticity gradient vanishes on this constant-$f_0$, constant-$N$, linear-shear basic state. Linear [advection](../../../../advection.md) of that perturbation therefore becomes $(\partial_t+\Lambda z\partial_x)q'=0$, the supplied interior equation. It retains slow balanced motion and omits [friction](../../../../friction.md), planetary-vorticity gradients and nonlinear disturbance [advection](../../../../advection.md).

Substitution of $\psi'=\Psi(z)\cos(ly)e^{ik(x-ct)}$ gives

$$
ik(\Lambda z-c)\left[\frac{f_0^2}{N^2}\Psi''-(k^2+l^2)\Psi\right]=0.
$$

A possible branch has zero interior perturbation [potential vorticity](../../../../potential-vorticity.md), so

$$
\boxed{\Psi''-K^2\Psi=0,\qquad
\Psi=A\cosh(Kz)+B\sinh(Kz),\qquad K=\frac{N\sqrt{k^2+l^2}}{|f_0|}}.
$$

Both supplied applications have $f_0>0$, so this equals the source's expression. For an unstable mode the nonzero [imaginary part](../../../../imaginary-part.md) of the [phase speed](../../../../phase-speed.md) prevents a real critical level $\Lambda z=c$; for real speeds the displayed solution remains a valid zero-interior-PV branch away from, and smoothly through, any critical level. Taking the [real part](../../../../real-part.md) gives the physical disturbance.

The rigid lids enforce $w'=0$. Linearized adiabatic [buoyancy](../../../../buoyancy.md) conservation is

$$
(\partial_t+\Lambda z\partial_x)b'+v'\bar b_y+N^2w'=0.
$$

Use the geostrophic conventions $v'=\psi'_x$ and $b'=f_0\psi'_z$. At a lid this gives $(\partial_t+\Lambda z\partial_x)\psi'_z-\Lambda\psi'_x=0$, hence

$$
\boxed{-c\Psi'(0)-\Lambda\Psi(0)=0,\qquad
(\Lambda H-c)\Psi'(H)-\Lambda\Psi(H)=0}.
$$

These are the no-normal-flow condition expressed through boundary [buoyancy](../../../../buoyancy.md) [advection](../../../../advection.md), not conditions of zero horizontal velocity. Boundary [temperature](../../../../temperature-split.md) anomalies can interact even though this solution has no interior perturbation PV, allowing [baroclinic instability](../../../../baroclinic-instability.md) to extract mean [available potential energy](../../../../available-potential-energy.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the physics of atmospheres and oceans course of the University of Oxford](../../../split.md)
5. [Physics of atmospheres and oceans course of the University of Oxford](../../../../physics-of-atmospheres-and-oceans-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
