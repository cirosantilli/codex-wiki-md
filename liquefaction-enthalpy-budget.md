# Liquefaction enthalpy budget

↑ **Parent:** [Helium liquefaction](helium-liquefaction.md)

Consider an original model of a cold section enclosing a throttle and collecting region, with the precooling [heat exchanger](heat-exchanger.md) outside its boundary. The inlet has [mass flow rate](mass-flow-rate.md) $\dot m>0$ and [specific enthalpy](specific-enthalpy.md) $h_{\rm in}$. The outlets are equilibrium [liquid](liquid.md) and [vapor](vapor.md) at one fixed [pressure](pressure-split.md), with [specific enthalpies](specific-enthalpy.md) $h_l$ and $h_g$. Let $y$ be the outlet [liquid](liquid.md) [mass fraction](mass-fraction.md), and let $q=\dot Q/\dot m\geq0$ be incoming unwanted [heat](heat-split.md) per unit incoming [mass](mass.md). Assume [steady flow](steady-flow.md), no shaft [work](work.md), and negligible bulk [kinetic energy](kinetic-energy.md) and [gravitational potential energy](gravitational-energy.md) changes. The [steady-flow energy balance](steady-flow-energy-balance.md) gives

$$
h_{\rm in}+q=yh_l+(1-y)h_g,\qquad
L=h_g-h_l>0,\qquad
y=\frac{h_g-h_{\rm in}-q}{L}.
$$

Here $L$ is the [latent heat](latent-heat.md) per unit [mass](mass.md) at the chosen outlet [pressure](pressure-split.md). The [mass flow rates](mass-flow-rate.md) of the outlets are $y\dot m$ and $(1-y)\dot m$. The formula describes a flowing cold section; a filling vessel with appreciable [energy](energy-split.md) or [mass](mass.md) accumulation requires storage terms.

For a deliberately dimensionless example, choose

$$
\eta=\frac{h_{\rm in}-h_l}{L}=0.70,\qquad
\ell=\frac qL=0.05,\qquad y=1-\eta-\ell=0.25.
$$

Per unit incoming [mass](mass.md), one quarter leaves as [liquid](liquid.md) and three quarters as [vapor](vapor.md). With zero incoming [heat](heat-split.md), the same inlet would give $y=0.30$. Increasing $q/L$ to $0.20$ reduces $y$ to $0.10$, and $q/L=0.30$ reaches the no-[liquid](liquid.md) boundary. These are chosen model values, not [helium](helium.md) property data or a historical yield. In normalized [enthalpy](enthalpy-split.md) units with $h_l=0$ and $h_g=1$, conservation checks directly: $0.70+0.05=0.25\times0+0.75\times1$.

<a id="liquefaction-enthalpy-fraction-model"></a>
![](liquefaction-enthalpy-fraction-model.png)

**[Figure 8](#liquefaction-enthalpy-fraction-model). An original normalized liquefaction enthalpy budget**. [Source](liquefaction-enthalpy-fraction-model.py). Each solid segment satisfies the stipulated equilibrium two-outlet model. Dashed negative continuations are algebra only: they do not describe a negative [liquid](liquid.md) [mass fraction](mass-fraction.md). No [helium](helium.md) properties or experimental measurements were fitted.

The admissible interval is $h_l\leq h_{\rm in}+q\leq h_g$, or $0\leq y\leq1$. Outside it, the assumed equilibrium two-phase outlet fails: an [enthalpy](enthalpy-split.md) above $h_g$ requires a hotter single-[vapor](vapor.md) outlet under these assumptions, rather than a negative amount of [liquid](liquid.md). Below $h_l$, a colder [liquid](liquid.md) or a different [thermodynamic phase](thermodynamic-phase.md) must be considered. The balance does not predict its own outlet [pressure](pressure-split.md), [temperature](temperature-split.md) or [helium](helium.md) property functions.

At fixed outlet [pressure](pressure-split.md), hence fixed $L$, the [derivatives](derivative.md) are $\partial y/\partial h_{\rm in}=-1/L$ and $\partial y/\partial q=-1/L$. Lowering inlet [specific enthalpy](specific-enthalpy.md) by regeneration and reducing incoming [heat](heat-split.md) therefore buy the same increase in [liquid](liquid.md) [mass fraction](mass-fraction.md) per unit [energy](energy-split.md) per unit [mass](mass.md) in this model. Adding any constant to all three [specific enthalpies](specific-enthalpy.md) leaves $y$ unchanged. This independence of the arbitrary [enthalpy](enthalpy-split.md) reference makes the balance useful even when property tables choose different zero points.

**Table of contents**

- [Liquefaction yield with separate warm-gas and liquid outlets](liquefaction-yield-with-separate-warm-gas-and-liquid-outlets.md)

## ↑ Ancestors (8)

1. [Helium liquefaction](helium-liquefaction.md)
2. [Cryogenics](cryogenics.md)
3. [Temperature](temperature-split.md)
4. [Thermodynamics](thermodynamics-split.md)
5. [Statistical physics](statistical-physics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Helium liquefaction](helium-liquefaction.md)
- [Liquefaction enthalpy budget](liquefaction-enthalpy-budget.md)
