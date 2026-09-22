<h1 id="stokes-s-law">Stokes's law</h1>

↑ **Parent:** [Surface traction in translating-sphere Stokes flow](surface-traction-in-translating-sphere-stokes-flow.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stokes's_law)

For an isolated rigid [sphere](sphere.md) of radius $a$ moving at [velocity](velocity.md) $\mathbf U$ relative to a distant uniform [Newtonian fluid](newtonian-fluid.md), the [drag force](drag-physics.md) exerted by the [fluid](fluid.md) is

$$
\mathbf F_D=-6\pi\mu a\mathbf U,\qquad |\mathbf F_D|=6\pi\mu aU.
$$

The assumptions are steady [incompressible flow](incompressible-flow.md), constant [dynamic viscosity](dynamic-viscosity-split.md) $\mu$, an unbounded surrounding [fluid](fluid.md), the [no-slip boundary condition](no-slip-boundary-condition.md), and a small diameter-based [particle Reynolds number](particle-reynolds-number.md), $\mathrm{Re}_d=2a\rho_fU/\mu\ll1$. Integrating the [surface traction in translating-sphere Stokes flow](surface-traction-in-translating-sphere-stokes-flow.md) gives the factor $6\pi$: the disturbance [pressure](pressure-split.md) contributes $2\pi\mu aU$ to the [drag](drag-physics.md) magnitude and the viscous [shear stress](shear-stress.md) contributes $4\pi\mu aU$. See [Richard Fitzpatrick, Axisymmetric Stokes Flow Around a Solid Sphere, equations 10.120–10.129](https://farside.ph.utexas.edu/teaching/336L/Fluid/node142.html).

The result is [linear drag](linear-drag.md): doubling $U$ doubles the [drag force](drag-physics.md), and doubling $a$ at fixed $U$ also doubles it. The required [power](power.md) is $6\pi\mu aU^2$, all supplied to [viscous dissipation](viscous-dissipation.md). [Density](density.md) enters the check of the [particle Reynolds number](particle-reynolds-number.md), although it does not appear in the leading [drag](drag-physics.md) formula.

Nearby walls or other particles change the [hydrodynamic resistance matrix](hydrodynamic-resistance-matrix.md) and invalidate the isolated-[sphere](sphere.md) coefficient, even at very small [Reynolds number](reynolds-number.md). Finite [Reynolds number](reynolds-number.md) introduces [inertia](inertia.md) corrections; the [Oseen approximation](oseen-approximation.md) resolves the distant region where the leading [Stokes flow](stokes-flow-split.md) approximation ceases to be uniform. A clean gas bubble has tangential slip and instead obeys [clean-bubble Stokes drag](clean-bubble-stokes-drag.md), with coefficient $4\pi\mu a$ in its spherical, negligible-internal-[viscosity](dynamic-viscosity-split.md) limit. See [H. K. Moffatt, Six Lectures on General Fluid Dynamics, section 3.4](https://www.damtp.cam.ac.uk/user/hkm2/PDFs/Moffatt_1977_GordonandBreach_Slogfdatohdt_149.pdf) for the [sphere](sphere.md) solution and its small-[Reynolds number](reynolds-number.md) limitation. The [continuum mechanics](continuum-mechanics-split.md) and boundary assumptions must also remain valid as the particle becomes very small.

Balancing this [Stokes drag law](stokes-s-law.md) against [gravity](gravity.md) and [buoyancy](buoyancy.md) gives the [Stokes settling velocity](stokes-settling-velocity.md) of an isolated rigid [sphere](sphere.md).

**Table of contents**

- [Rarefied-gas nanoparticle drag](rarefied-gas-nanoparticle-drag.md)
- [Particle velocity-relaxation time](particle-velocity-relaxation-time.md)
- [Gas slip correction to Stokes drag](gas-slip-correction-to-stokes-drag.md)
- [Clean-bubble Stokes drag](clean-bubble-stokes-drag.md)
  - [Bubble rise near a distant stress-free free surface](bubble-rise-near-a-distant-stress-free-free-surface.md)
  - [Spherical clean bubble without surface tension](spherical-clean-bubble-without-surface-tension.md)
- [Stokes–Einstein relation](stokes-einstein-relation.md)
  - [Brownian radius estimate from endpoint displacements](brownian-radius-estimate-from-endpoint-displacements.md)
    - [Sampling uncertainty of an endpoint diffusivity estimate](sampling-uncertainty-of-an-endpoint-diffusivity-estimate.md)
  - [Stokes-Einstein experimental consistency test](stokes-einstein-experimental-consistency-test.md)

## ↑ Ancestors (7)

1. [Surface traction in translating-sphere Stokes flow](surface-traction-in-translating-sphere-stokes-flow.md)
2. [Stokes flow](stokes-flow-split.md)
3. [Viscous fluid flow](viscous-fluid-flow-split.md)
4. [Fluid mechanics](fluid-mechanics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (12)

- [Elementary charge](elementary-charge.md)
- [Finite-time rate-zonal separation](finite-time-rate-zonal-separation.md)
- [Gas slip correction to Stokes drag](gas-slip-correction-to-stokes-drag.md)
- [Mechanical mobility](mechanical-mobility.md)
- [Molar mass from sedimentation and diffusion](molar-mass-from-sedimentation-and-diffusion.md)
- [Solution](past-exam-of-the-mathematical-and-computational-biology-course-of-the-university-of-cambridge/2025/paper-2/7/b/solution.md)
- [Solution](past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2018/section-a/1/b/solution.md)
- [Solution](past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2019/section-b/b4/solution.md)
- [Rate-zonal centrifugation](rate-zonal-centrifugation.md)
- [Sedimentation coefficient](sedimentation-coefficient.md)
- [Stokes flow](stokes-flow-split.md)
- [Velocity relaxation time](velocity-relaxation-time.md)
