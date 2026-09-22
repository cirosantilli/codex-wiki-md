# Momentum thickness

↑ **Parent:** [Boundary layer thickness](boundary-layer-thickness.md)

The [momentum thickness](momentum-thickness.md) weights the streamwise [velocity](velocity.md) deficit by the local [velocity](velocity.md) carrying it:

$$
\theta=\int_0^\infty\frac{u}{U}\left(1-\frac{u}{U}\right)\,dy,\qquad \rho U^2\theta=\rho\int_0^\infty u(U-u)\,dy.
$$

Thus $\rho U^2\theta$ measures a [momentum flux](momentum-flux.md) deficit per unit span relative to transporting the same local [mass flow rate](mass-flow-rate.md) at $U$. It is not $\rho\int(U^2-u^2)\,dy$, which compares a different reference flux. A [Blasius boundary layer](blasius-boundary-layer.md) has $\theta\simeq0.664115\sqrt{\nu x/U}$; the ratio of [displacement thickness](displacement-thickness.md) to [momentum thickness](momentum-thickness.md) is about $2.591$.[Boundary-layer Thickness, Skin friction, and Energy dissipation](modules-on-high-reynolds-number-flows/boundary-layer-thickness-skin-friction-and-energy-dissipation.md)

For the [steady flow](steady-flow.md) over an impermeable flat plate at constant $U$, integrating the [boundary-layer equation](boundary-layer-equation.md) and using [mass conservation](mass-conservation.md) gives

$$
\frac{d\theta}{dx}=\frac{\tau_w}{\rho U^2}.
$$

This connects growth of the [momentum thickness](momentum-thickness.md) to local [wall shear stress](wall-shear-stress.md). Consequently the [drag](drag-physics.md) per unit span on one face up to $x=L$ is $D'=\rho U^2\theta(L)$ in the ideal [Blasius boundary layer](blasius-boundary-layer.md) with $\theta(0)=0$. Measured [velocity profiles](velocity-profile.md) can therefore estimate integrated [drag](drag-physics.md) without differentiating noisy near-wall readings. The identity assumes no wall suction and zero outer [pressure gradient](pressure-gradient.md).[Momentum Integral](modules-on-high-reynolds-number-flows/momentum-integral.md)

## ↑ Ancestors (6)

1. [Boundary layer thickness](boundary-layer-thickness.md)
2. [Boundary layer](boundary-layer.md)
3. [Continuum mechanics](continuum-mechanics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Boundary layer thickness](boundary-layer-thickness.md)
- [Flat-plate boundary-layer traverse experiment](flat-plate-boundary-layer-traverse-experiment.md)
- [Momentum thickness](momentum-thickness.md)
