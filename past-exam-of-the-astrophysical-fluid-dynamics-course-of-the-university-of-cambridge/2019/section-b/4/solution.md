<h1 id="section-b/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

**Following a fluid element.** Let $\mathbf X(t)$ be a [pathline](../../../../pathline.md), satisfying $\dot{\mathbf X}=\mathbf u(\mathbf X,t)$. The [material derivative](../../../../material-derivative.md), also called the Lagrangian time derivative, is the rate observed while following that element. The [multivariable chain rule](../../../../multivariable-chain-rule.md) gives

$$
\boxed{\frac{D\phi}{Dt}=\frac{d}{dt}\phi(\mathbf X(t),t)
=\frac{\partial\phi}{\partial t}+\mathbf u\cdot\nabla\phi.}
$$

The [partial derivative](../../../../partial-derivative.md) holds position fixed; the [advection](../../../../advection.md) term accounts for motion through a spatially varying field. For a [vector field](../../../../vector-field.md), the same formula applies component by component in fixed Cartesian axes.

**Momentum balance.** For an [inviscid flow](../../../../inviscid-flow.md), [pressure](../../../../pressure-split.md) is the only surface stress. A small material volume $dV$ has net pressure [force](../../../../force-split.md) $-\nabla p\,dV$, obtained by the [divergence theorem](../../../../divergence-theorem.md). Its [mass](../../../../mass.md) is $\rho\,dV$ and its [material acceleration](../../../../material-acceleration.md) is $D\mathbf u/Dt$. Applying [Newton's second law](../../../../newton-s-second-law.md) gives the [Euler equations for an inviscid fluid](../../../../euler-equations-for-an-inviscid-fluid-split.md),

$$
\boxed{\rho\frac{D\mathbf u}{Dt}
=\rho\left[\partial_t\mathbf u+(\mathbf u\cdot\nabla)\mathbf u\right]
=-\nabla p.}
$$

This is the local [momentum conservation](../../../../momentum-conservation.md) equation when viscosity and physical [body forces](../../../../body-force.md) are absent. A prescribed [body force](../../../../body-force.md) per unit mass would add $\rho\mathbf f$ on the right.

**Changing to rotating coordinates.** In a [rotating frame](../../../../rotating-reference-frame.md) with constant [angular velocity](../../../../angular-velocity.md) $\boldsymbol\Omega$, the lab acceleration is the rotating-frame [material acceleration](../../../../material-acceleration.md) plus $2\boldsymbol\Omega\times\mathbf u+\boldsymbol\Omega\times(\boldsymbol\Omega\times\mathbf r)$. Therefore

$$
\rho_0\left[\partial_t\mathbf u+(\mathbf u\cdot\nabla)\mathbf u
+2\boldsymbol\Omega\times\mathbf u\right]
=-\nabla p-\rho_0\boldsymbol\Omega\times(\boldsymbol\Omega\times\mathbf r).
$$

For uniform rotation,

$$
\boldsymbol\Omega\times(\boldsymbol\Omega\times\mathbf r)
=-\nabla\!\left(\frac12|\boldsymbol\Omega\times\mathbf r|^2\right).
$$

With constant $\rho_0$, this gives the [Euler equation in a uniformly rotating frame](../../../../euler-equation-in-a-uniformly-rotating-frame.md),

$$
\boxed{\rho_0\left[\partial_t\mathbf u+2\boldsymbol\Omega\times\mathbf u
+(\mathbf u\cdot\nabla)\mathbf u\right]
=-\nabla\!\left[p-\frac{\rho_0}{2}|\boldsymbol\Omega\times\mathbf r|^2\right].}
$$

The term subtracted from $p$ is the equilibrium centrifugal contribution. Dividing the bracket by $\rho_0$ defines a reduced pressure $\Pi=p/\rho_0-|\boldsymbol\Omega\times\mathbf r|^2/2$, with units $\mathrm{m^2\,s^{-2}}$. The [Coriolis acceleration](../../../../coriolis-acceleration.md) remains a velocity-dependent term.

**Linear disturbances.** Linearize about rest in the rotating coordinates, with the equilibrium part of $\Pi$ removed. The advective acceleration is quadratic in disturbance amplitude, so the [linearized Euler equations](../../../../linearized-euler-equations.md) and [incompressible flow](../../../../incompressible-flow.md) condition are

$$
\partial_t\mathbf u+2\boldsymbol\Omega\times\mathbf u=-\nabla\Pi',\qquad
\nabla\cdot\mathbf u=0.
$$

Taking the [curl](../../../../curl.md) removes the pressure [gradient](../../../../gradient.md). The identity

$$
\nabla\times(\boldsymbol\Omega\times\mathbf u)
=\boldsymbol\Omega(\nabla\cdot\mathbf u)-(\boldsymbol\Omega\cdot\nabla)\mathbf u
=-(\boldsymbol\Omega\cdot\nabla)\mathbf u
$$

gives the [inertial-wave vorticity equation](../../../../inertial-wave-vorticity-equation.md),

$$
\boxed{\partial_t(\nabla\times\mathbf u)-2(\boldsymbol\Omega\cdot\nabla)\mathbf u=0,
\qquad \nabla\cdot\mathbf u=0.}
$$

**Plane-wave frequencies.** Let $\mathbf k\ne0$ and use the given [plane wave](../../../../plane-wave.md) convention. [Incompressible flow](../../../../incompressible-flow.md) requires $\mathbf k\cdot\mathbf u_0=0$, and the [vorticity](../../../../vorticity-split.md) equation gives

$$
\omega\,\mathbf k\times\mathbf u_0
=2i(\boldsymbol\Omega\cdot\mathbf k)\mathbf u_0.
$$

For a nonzero frequency, apply $\mathbf k\times$ again, using $\mathbf k\times(\mathbf k\times\mathbf u_0)=-k^2\mathbf u_0$. It follows that

$$
\boxed{\omega^2=\frac{4(\boldsymbol\Omega\cdot\mathbf k)^2}{k^2}
=4\Omega^2\frac{k_z^2}{k^2},\qquad \omega=\pm2\Omega\frac{k_z}{k}.}
$$

This is the [inertial-wave dispersion relation](../../../../inertial-wave-dispersion-relation.md). If $\theta$ is the angle of the [wavevector](../../../../wavevector.md) to the rotation axis, the positive [angular frequency](../../../../angular-frequency.md) is $2|\Omega\cos\theta|$. It is largest, $2|\Omega|$, for a parallel [wavevector](../../../../wavevector.md), decreases to zero for a perpendicular one, and is independent of the magnitude of the [wavenumber](../../../../wavenumber.md) at fixed direction. The two signs describe the two oscillatory polarization branches. When $k_z=0$, the zero-frequency result is obtained directly from the linear equations rather than by dividing by $\omega$; it describes the nonoscillating balanced limit.

## ↑ Ancestors (13)

1. [4](../4.md)
2. [Section B](../../section-b.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the astrophysical fluid dynamics course of the University of Cambridge](../../../split.md)
5. [Astrophysical Fluid Dynamics course of the University of Cambridge](../../../../astrophysical-fluid-dynamics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
