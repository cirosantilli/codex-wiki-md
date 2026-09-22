<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The [Hiemenz flow](../../../../hiemenz-flow.md) profile changes on $\eta=O(1)$, so its [boundary layer thickness](../../../../boundary-layer-thickness.md) is

$$
\boxed{\delta_{\mathrm{BL}}\sim\sqrt{\frac\nu A}.}
$$

A specified edge convention, such as $u/(Ax)=0.99$, introduces an order-one numerical multiplier requiring the profile to be solved. Scaling alone does not determine that multiplier. The result has no separate dependence on $x$, $y$, $\rho$ or $p_0$ at fixed [kinematic viscosity](../../../../kinematic-viscosity.md). At fixed [dynamic viscosity](../../../../dynamic-viscosity-split.md), it is $\sqrt{\eta/(\rho A)}$.

The [viscous diffusion time](../../../../viscous-diffusion-time.md) across a thickness $\delta$ is $\delta^2/\nu$; the imposed strain has time scale $A^{-1}$. Their balance sets the thickness. Increasing [kinematic viscosity](../../../../kinematic-viscosity.md) spreads the layer, while increasing the imposed [velocity gradient](../../../../velocity-gradient.md) presses the layer toward the wall. The outward tangential [velocity](../../../../velocity.md) increases as $Ax$, so the decreasing travel time per unit distance offsets the usual downstream broadening.

For a conventional estimate of transition to [turbulence](../../../../turbulence-split.md), form the local horizontal [Reynolds number](../../../../reynolds-number.md):

$$
\mathrm{Re}_x=\frac{(Ax)x}{\nu}=\frac{Ax^2}{\nu}.
$$

If transition is assumed to occur at an empirical value $\mathrm{Re}_{\mathrm{crit}}$, then

$$
\boxed{l\sim\sqrt{\frac{\mathrm{Re}_{\mathrm{crit}}\nu}{A}}.}
$$

A rough borrowed threshold of order $10^5$–$10^6$ would give $l$ of order $10^2$–$10^3\sqrt{\nu/A}$. This is a heuristic estimate, not a universal stability prediction: the accelerating outer flow and favorable [pressure gradient](../../../../pressure-gradient.md) can delay transition, and disturbance amplitudes and wall roughness matter. Simply setting $\mathrm{Re}_x\sim1$ locates failure of the thin-layer approximation near the [stagnation point](../../../../stagnation-point.md), not onset of [turbulence](../../../../turbulence-split.md).

## ↑ Ancestors (12)

1. [E](../e.md)
2. [2](../../2.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the fluids course of the University of Oxford](../../../split.md)
5. [Fluids course of the University of Oxford](../../../../fluids-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
