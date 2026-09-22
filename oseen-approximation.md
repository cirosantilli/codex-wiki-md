# Oseen approximation

↑ **Parent:** [Stokes flow](stokes-flow-split.md)

The [Oseen approximation](oseen-approximation.md) retains [advection](advection.md) of a small disturbance by a uniform incident [velocity](velocity.md) $\mathbf U$, but neglects [advection](advection.md) of the disturbance by itself. Its steady equations are

$$
\rho(\mathbf U\cdot\nabla)\mathbf u=-\nabla p+\mu\nabla^2\mathbf u,\qquad\nabla\cdot\mathbf u=0.
$$

A Stokes disturbance of a [sphere](sphere.md) decays as $Ua/r$, so the ratio of background [advection](advection.md) to viscous [diffusion](diffusion.md) grows as $Ur/\nu$. Thus the approximation resolves the outer region $r\sim\nu/U$, where the [Stokes flow](stokes-flow-split.md) expansion is nonuniform, while self-convection remains smaller by $a/r$.

**Table of contents**

- [Potential-source and wake decomposition of sphere Oseen flow](potential-source-and-wake-decomposition-of-sphere-oseen-flow.md)

## ↑ Ancestors (6)

1. [Stokes flow](stokes-flow-split.md)
2. [Viscous fluid flow](viscous-fluid-flow-split.md)
3. [Fluid mechanics](fluid-mechanics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Oseen approximation](oseen-approximation.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-86/3/solution.md)
