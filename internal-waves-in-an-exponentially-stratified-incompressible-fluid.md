# Internal waves in an exponentially stratified incompressible fluid

↑ **Parent:** [Internal wave](internal-wave.md)

For a quiescent two-dimensional incompressible inviscid fluid with [mass density](density.md) $\rho_0(z)=r e^{-\alpha z}$ and $\alpha>0$, [hydrostatic balance](hydrostatic-balance.md) and density advection give the linear perturbation equations

$$
u_x+w_z=0,\quad \rho_0u_t=-p_x,\quad \rho_0w_t=-p_z-g\rho',\quad \rho'_t=\alpha\rho_0w.
$$

Eliminating [pressure](pressure-split.md) and density perturbations gives the title [partial differential equation](partial-differential-equation-split.md). It retains the variation of inertial density rather than invoking the [Boussinesq approximation](boussinesq-approximation.md). The transformation $w=e^{\alpha z/2}W$ gives $\partial_t^2(\nabla^2W-\alpha^2W/4)+\alpha gW_{xx}=0$. Between rigid boundaries at $z=0,h$, the [normal modes](normal-mode.md) have

$$
W\propto\sin(n\pi z/h)e^{i(kx-\omega t)},\qquad \omega^2=\frac{\alpha gk^2}{k^2+(n\pi/h)^2+\alpha^2/4},\quad n\geq1.
$$

The vertical [velocity](velocity.md) is $e^{\alpha z/2}W$; the exponential factor compensates for the decreasing background [mass density](density.md) in the mode structure.

**Table of contents**

- [Horizontal group-speed bound for a confined internal wave](horizontal-group-speed-bound-for-a-confined-internal-wave.md)

## ↑ Ancestors (6)

1. [Internal wave](internal-wave.md)
2. [Gravity wave](gravity-wave-split.md)
3. [Fluid mechanics](fluid-mechanics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-waves-and-compressible-flow-course-of-the-university-of-oxford/2023/2/a/i/solution.md)
