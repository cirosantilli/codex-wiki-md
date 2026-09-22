# Steady-flow energy balance

↑ **Parent:** [Enthalpy](enthalpy-split.md)

For [steady flow](steady-flow.md) through a fixed [control volume](control-volume.md) with one inlet and one outlet, the [first law of thermodynamics](first-law-of-thermodynamics-split.md) and conservation of [mass](mass.md) give

$$
\dot Q-\dot W_s=\dot m\left[h_2-h_1+\frac{w_2^2-w_1^2}{2}+g(z_2-z_1)\right].
$$

Here $\dot m$ is the [mass flow rate](mass-flow-rate.md), $\dot Q$ incoming [heat](heat-split.md) per unit time, $\dot W_s$ outgoing non-flow [work](work.md) per unit time, $w$ the flow speed, $z$ elevation and $g$ [gravitational acceleration](gravitational-acceleration.md). The [specific enthalpy](specific-enthalpy.md) $h=u+p/\rho$ includes both the transported [internal energy](internal-energy-split.md) per unit [mass](mass.md) $u$ and the [pressure](pressure-split.md) [work](work.md) needed to push [volume](volume-thermodynamics.md) through the boundary; $\rho$ is [mass density](density.md). The inlet supplies that [pressure](pressure-split.md) [work](work.md), while the outlet consumes it to displace the downstream [fluid](fluid.md).[§2.5.1–2.5.2, equation 2.11: mass conservation, transported enthalpy and the steady-flow energy equation](thermodynamics-and-propulsion.md)

For an insulated stationary throttle, require negligible [heat](heat-split.md) transfer, no shaft or other non-flow [work](work.md), and negligible changes in bulk [kinetic energy](kinetic-energy.md) and gravitational [potential energy](potential-energy.md). Then $h_2=h_1$. With unchanged composition this is also equality of [molar enthalpy](molar-enthalpy.md). The upstream and downstream states must admit equilibrium [pressure](pressure-split.md), [temperature](temperature-split.md) and property values, although the constriction itself is irreversible and can be far from [thermodynamic equilibrium](thermodynamic-equilibrium.md). Start-up storage of [energy](energy-split.md) in the walls and [fluid](fluid.md), heat leakage, or a large outlet speed invalidates the reduced balance. A nozzle can convert [specific enthalpy](specific-enthalpy.md) into bulk [kinetic energy](kinetic-energy.md) even when it is insulated.

The same accounting for a fixed transported amount is $U_2-U_1=p_1V_1-p_2V_2$, hence $U_1+p_1V_1=U_2+p_2V_2$. This explains why dropping the two [pressure](pressure-split.md) [work](work.md) terms would give the wrong conserved quantity.[Fitzpatrick, Joule-Thompson Throttling, equations 6.167–6.174: inlet/outlet pressure work and enthalpy conservation](thermodynamics-and-statistical-mechanics-by-richard-fitzpatrick/joule-thompson-throttling.md)

## ↑ Ancestors (6)

1. [Enthalpy](enthalpy-split.md)
2. [Thermodynamics](thermodynamics-split.md)
3. [Statistical physics](statistical-physics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Helium liquefaction](helium-liquefaction.md)
- [Isenthalpic process](isenthalpic-process.md)
- [Joule-Thomson coefficient](joule-thomson-coefficient.md)
- [Joule-Thomson effect](joule-thomson-effect.md)
- [Liquefaction enthalpy budget](liquefaction-enthalpy-budget.md)
- [Liquefaction yield with separate warm-gas and liquid outlets](liquefaction-yield-with-separate-warm-gas-and-liquid-outlets.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2013/paper-2/section-c/c11/solution.md)
- [Van der Waals throttling model](van-der-waals-throttling-model.md)
