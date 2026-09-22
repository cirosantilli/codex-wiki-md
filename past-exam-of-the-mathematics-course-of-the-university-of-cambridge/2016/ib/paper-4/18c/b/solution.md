<h1 id="18c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For constant density $\rho$ and constant angular velocity $\boldsymbol\Omega$, the [Euler equations for an inviscid fluid](../../../../../../euler-equations-for-an-inviscid-fluid.md) in the rotating frame is

$$
\partial_t\mathbf u+(\mathbf u\cdot\nabla)\mathbf u+2\boldsymbol\Omega\times\mathbf u=-\frac1\rho\nabla p-\nabla\Phi_g-\boldsymbol\Omega\times(\boldsymbol\Omega\times\mathbf r),\qquad\nabla\cdot\mathbf u=0.
$$

The last two forces are gravity and [centrifugal acceleration](../../../../../../centrifugal-acceleration.md); $2\boldsymbol\Omega\times\mathbf u$ is the [Coriolis force](../../../../../../coriolis-force.md) term on the left. Incorporate both conservative forces into the modified pressure

$$
\Pi=p/\rho+\Phi_g-\tfrac12|\boldsymbol\Omega\times\mathbf r|^2,
$$

so the right side is $-\nabla\Pi$.

At latitude $\lambda$ on a spherical Earth of radius $R$, the outward local vertical component of [centrifugal acceleration](../../../../../../centrifugal-acceleration.md) is $\Omega_E^2R\cos^2\lambda$. Its ratio to gravity is at most $\Omega_E^2R/g\simeq3.5\times10^{-3}$, using $\Omega_E\simeq7.3\times10^{-5}\,\mathrm{s}^{-1}$, $R\simeq6.4\times10^6\,\mathrm m$, and $g\simeq9.8\,\mathrm{m\,s}^{-2}$. Thus this component is small compared with gravity everywhere on Earth.

For a velocity scale $U$ and length scale $\ell$, nonlinear advection scales as $U^2/\ell$, whereas the Coriolis term scales as $2\Omega U$. Their ratio is the [Rossby number](../../../../../../rossby-number.md) $U/(2\Omega\ell)$. If it is small, for example by increasing rotation at fixed $U,\ell$, neglect nonlinear advection in perturbations about a fluid at rest. The conservative equilibrium forces have already been absorbed into pressure; with a rotation-timescale unsteady motion the leading equations are

$$
\boxed{\partial_t\mathbf u+2\boldsymbol\Omega\times\mathbf u=-\nabla\Pi',\qquad\nabla\cdot\mathbf u=0.}
$$

These are the linear equations governing [inertial waves](../../../../../../inertial-wave.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [18C](../../18c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
