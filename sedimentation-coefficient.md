# Sedimentation coefficient

↑ **Parent:** [Centrifugation](centrifugation.md)

The [sedimentation coefficient](sedimentation-coefficient.md) $s$ is radial drift [velocity](velocity.md) divided by local [centrifugal acceleration](centrifugal-acceleration.md). It has units of time and combines particle properties with those of the surrounding liquid. In a dilute, deterministic [mathematical model](mathematical-model.md) with negligible particle [inertia](inertia.md), an effective displaced volume $V$, particle [mass](mass.md) $m$, local liquid [density](density.md) $\rho_f$ and [linear friction coefficient](linear-friction-coefficient.md) $f>0$ give

$$
f v=(m-\rho_f V)\omega^2r,\qquad s=\frac{v}{\omega^2r}=\frac{m-\rho_f V}{f}.
$$

The subtraction represents [buoyancy](buoyancy.md). Equal [mass](mass.md) does not imply equal $s$: changing shape changes [drag force](drag-physics.md), and changing the medium changes both [buoyancy](buoyancy.md) and [viscosity](dynamic-viscosity.md).[An Introduction to Ultracentrifugation, The Physics Behind the Technology: mass, size, shape, medium density and viscosity](https://www.beckman.com/resources/technologies/centrifugation/ultracentrifugation/)

For an isolated [sphere](sphere.md) of radius $b$ and uniform [density](density.md) $\rho_p$, [Stokes's law](stokes-s-law.md) supplies $f=6\pi\eta b$, where $\eta$ is dynamic [viscosity](dynamic-viscosity.md), and $m=(4\pi/3)b^3\rho_p$. Therefore

$$
s=\frac{2b^2(\rho_p-\rho_f)}{9\eta}.
$$

This original force-balance check predicts fourfold $s$ on doubling $b$ with everything else fixed, and zero drift when $\rho_p=\rho_f$. It applies to dilute isolated [spheres](sphere.md) in [Stokes flow](stokes-flow-split.md), not arbitrary folded [proteins](protein.md) or crowded suspensions. If $s$ and $\omega$ remain constant in a uniform medium, the [ordinary differential equation](ordinary-differential-equation.md) $dr/dt=s\omega^2r$ has the [exponential function](exponential-function.md) solution $r(t)=r(0)e^{s\omega^2t}$. Arrival at an outer boundary therefore depends on starting position as well as $s$; a separation has no universal size cutoff.

## ↑ Ancestors (3)

1. [Centrifugation](centrifugation.md)
2. [Biology](biology-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Centrifugation](centrifugation.md)
- [Rate-zonal centrifugation](rate-zonal-centrifugation.md)
- [Sedimentation coefficient](sedimentation-coefficient.md)
