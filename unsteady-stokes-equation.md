# Unsteady Stokes equation

↑ **Parent:** [Stokes equation](stokes-equation.md)

For variations on a time scale $T$, the ratio of local [inertia](inertia.md) to viscous resistance is $L^2/(\nu T)$. Steady [Stokes flow](stokes-flow-split.md) at each instant requires both $UL/\nu\ll1$ and $L^2/(\nu T)\ll1$. If only the first is small, retain local [acceleration](acceleration.md):

$$
\rho\frac{\partial\mathbf u}{\partial t}=-\nabla p+\mu\nabla^2\mathbf u+\mathbf f,\qquad \nabla\cdot\mathbf u=0.
$$

For an oscillating [sphere](sphere.md) with angular frequency $\omega$, the second condition becomes $\omega a^2/\nu\ll1$ on the radius scale $a$. The [Unsteady Stokes equation](unsteady-stokes-equation.md) is still linear, but needs initial data and has memory; its [velocity field](velocity-field.md) is not determined by instantaneous boundary [velocities](velocity.md) alone. See [E. J. Hinch, Slow Viscous Flow, example sheet 1, question 1](https://www.damtp.cam.ac.uk/user/coflu/teaching/eg1-2008.pdf) for the distinction between steady and unsteady limits of an oscillating [sphere](sphere.md).

## ↑ Ancestors (7)

1. [Stokes equation](stokes-equation.md)
2. [Stokes flow](stokes-flow-split.md)
3. [Viscous fluid flow](viscous-fluid-flow-split.md)
4. [Fluid mechanics](fluid-mechanics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Stokes flow](stokes-flow-split.md)
- [Stokes settling velocity](stokes-settling-velocity.md)
- [Unsteady Stokes equation](unsteady-stokes-equation.md)
