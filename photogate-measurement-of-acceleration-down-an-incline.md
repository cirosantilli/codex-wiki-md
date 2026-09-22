# Photogate measurement of acceleration down an incline

↑ **Parent:** [Inclined plane](inclined-plane.md)

A modern teaching experiment slows gravity-driven motion enough to resolve it with a [photogate](photogate.md). PASCO scientific's [Inclined Plane Dynamics Set, ME-6966, Instruction Manual 012-10874A](https://cdn.pasco.com/product_document/Inclined-Plane-Dynamics-Set-Manual-ME-6966.pdf) describes “Acceleration Down an Incline” on printed pages 15–16. Its apparatus is a GOcar on a PAStrack with an adjustable incline support, a bracket-mounted [photogate](photogate.md), a cart-mounted picket fence, and an interface with recording software. For the interface method, the fence's $1\,\mathrm{cm}$ pattern is aligned to interrupt the beam. Recording starts before release from rest; the cart is caught at the bottom bumper. The procedure specifies three runs per [angle](angle.md), starting at $14^\circ$ and reducing by $2^\circ$, with the release [position](position.md) fixed. The readout is [velocity](velocity.md) against [time](time-in-physics.md); its slope estimates [acceleration](acceleration.md). Mean [accelerations](acceleration.md) are plotted against $\sin\theta$, testing the ideal slope $g$. An added-[mass](mass.md) comparison is also requested. These are protocol settings, not observed results.[Printed pp. 15–16, equipment, procedure steps 1–8, analysis steps 1–3 and question 2; interface timing note](inclined-plane-dynamics-set-me-6966-instruction-manual-012-10874a-by-pasco-scientific.md)

The cart undergoes [rolling without slipping](rolling-without-slipping.md) at its wheels, whereas the worked block undergoes [contact slip](contact-slip.md). Even ideal wheel [moment of inertia](moment-of-inertia.md) changes the cart prediction. For total cart [mass](mass.md) $M$, wheel radii $r_i$ and axial [moments of inertia](moment-of-inertia.md) $I_i$, rigid wheels with fixed axles and no losses give

$$
a=\frac{g\sin\theta}{1+\displaystyle\sum_i I_i/(Mr_i^2)}.
$$

To derive it, combine translational [kinetic energy](kinetic-energy.md) $Mv^2/2$ with wheel [rotational kinetic energy](rotational-kinetic-energy.md) $\sum_i I_i(v/r_i)^2/2$, then equate their rate of change to the release of [gravitational potential energy](gravitational-energy.md) $Mg\sin\theta\,v$. This is the multiwheel counterpart of [rolling acceleration with rotational inertia](rolling-acceleration-with-rotational-inertia.md). Neglecting wheel [moment of inertia](moment-of-inertia.md) yields $a\simeq g\sin\theta$; treating a cart as a solid rolling cylinder would give a different correction.

Useful additional controls are repeated releases without a push, checking the fence alignment and spacing, and checking that the recorded [velocity](velocity.md) trace is straight over the fitted interval. A gently moving cart on a level track can expose losses or unintended tilt. These checks help distinguish an [angle](angle.md) or timing error from neglected wheel [moment of inertia](moment-of-inertia.md), bearing [friction](friction.md), or [drag force](drag-physics.md). The three-run spread measures repeatability but cannot by itself reveal a shared calibration error. The inspected protocol makes the gravity component measurable; it does not measure the sliding block's [coefficient of kinetic friction](coefficient-of-kinetic-friction.md).

## ↑ Ancestors (5)

1. [Inclined plane](inclined-plane.md)
2. [Classical mechanics](classical-mechanics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)
