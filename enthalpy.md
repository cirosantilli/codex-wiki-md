# Enthalpy

↑ **Parent:** [Thermodynamics](thermodynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Enthalpy)

Enthalpy is the [state function](thermodynamics.md#state-function) obtained by adding [pressure](pressure.md) times [volume](thermodynamics.md#volume-thermodynamics) to [internal energy](internal-energy.md):

$$
H=U+pV.
$$

Here $U$ denotes [internal energy](internal-energy.md), also written $E$ in some references. Like [internal energy](internal-energy.md), [enthalpy](enthalpy.md) is measured in [joules](physics.md#joule) and is an [extensive variable](thermodynamics.md#extensive-quantity). Its definition packages the [internal energy](internal-energy.md) change and expansion [work](energy.md#work) into one useful quantity for fixed-[pressure](pressure.md) calculations. It does not define a body's stored [heat](heat.md). [IUPAC Gold Book, enthalpy](https://goldbook.iupac.org/terms/view/E02141/plain)

For a fixed amount and composition of a [simple compressible system](thermodynamics.md#simple-compressible-system), the relation between neighboring equilibrium states is

$$
dH=T\,dS+V\,dp.
$$

Here $T$ is absolute [temperature](temperature.md) and $S$ is [entropy](entropy.md). Thus [entropy](entropy.md) and [pressure](pressure.md) are the natural variables of this [thermodynamic potential](thermodynamic-potential.md), with [partial derivatives](multivariable-calculus.md#partial-derivative) $T=(\partial H/\partial S)_p$ and $V=(\partial H/\partial p)_S$. Fixed composition matters: changing composition adds further terms. The formula follows in one line from the equilibrium [first law of thermodynamics](first-law-of-thermodynamics.md) identity:

$$
dH=dU+p\,dV+V\,dp=(T\,dS-p\,dV)+p\,dV+V\,dp=T\,dS+V\,dp.
$$

The cancellation of $p\,dV$ is the reason [enthalpy](enthalpy.md) replaces [volume](thermodynamics.md#volume-thermodynamics) with [pressure](pressure.md) as a natural variable. This identity concerns equilibrium states; it does not identify $T\,dS$ with actual irreversible [heat](heat.md) transfer. [David Tong, Statistical Physics, section 4.4.1: enthalpy](https://davidtong.org/teaching/statistical-physics/statmechhtml/S4#S4.SS4.SSS1)

For a [closed system](thermodynamics.md#closed-system) undergoing a [quasistatic process](thermodynamics.md#quasistatic-process) at constant [pressure](pressure.md), require fixed amount and composition, only [pressure](pressure.md)-[volume](thermodynamics.md#volume-thermodynamics) [work](energy.md#work), no [friction](newtonian-mechanics.md#friction), and unchanged bulk [kinetic energy](energy.md#kinetic-energy) and [potential energy](energy.md#potential-energy). Then the actual [first law of thermodynamics](first-law-of-thermodynamics.md) balance gives

$$
\delta Q=dU+p\,dV=dH-V\,dp,\qquad
dp=0\ \Longrightarrow\ Q_p=\Delta H.
$$

The symbol $Q_p$ means transferred [heat](heat.md) for this fixed-[pressure](pressure.md) process. If the piston example in [heat](heat.md) additionally meets these conditions, its $20\,\mathrm{kJ}$ of incoming [heat](heat.md) equals $\Delta H$, while $\Delta U=15\,\mathrm{kJ}$ and $p\Delta V=W=5\,\mathrm{kJ}$. The example shows exactly what [enthalpy](enthalpy.md) adds to [internal energy](internal-energy.md): the expansion [work](energy.md#work) required at the imposed [pressure](pressure.md).

Within a single [thermodynamic phase](thermodynamics.md#thermodynamic-phase), [heat capacity at constant pressure](#heat-capacity-at-constant-pressure) gives

$$
C_p=\left(\frac{\partial H}{\partial T}\right)_p,\qquad
\Delta H=\int_{T_1}^{T_2}C_p(T)\,dT
$$

with the amount and composition fixed. Constant $C_p$ gives $\Delta H=C_p\Delta T$; dividing by [mass](classical-mechanics.md#mass) gives [specific heat capacity at constant pressure](heat.md#specific-heat-capacity-at-constant-pressure). At equilibrium [melting](critical-phenomenon.md#melting), [enthalpy](enthalpy.md) can instead change through [latent heat](thermodynamic-potential.md#latent-heat) while [temperature](temperature.md) stays fixed. The [sensible heat](heat.md#sensible-heat) example therefore adds two single-[thermodynamic phase](thermodynamics.md#thermodynamic-phase) [enthalpy](enthalpy.md) changes and one [latent heat](thermodynamic-potential.md#latent-heat) contribution.

The usefulness of [enthalpy](enthalpy.md) lies in matching the imposed constraint: a fixed-[pressure](pressure.md) experiment naturally reports $\Delta H$, while fixed-[volume](thermodynamics.md#volume-thermodynamics) heating with no other [work](energy.md#work) reports $\Delta U$. Neither equality is universal. Additional [work](energy.md#work) or changing [pressure](pressure.md) alters the relation between supplied [heat](heat.md) and $\Delta H$; irreversible [entropy](entropy.md) production also prevents identifying actual $\delta Q$ with $T\,dS$. The separate [Joule-Thomson coefficient](#joule-thomson-coefficient) branch uses [enthalpy](enthalpy.md) to describe throttling under its own assumptions.

**Table of contents**

- [Stagnation enthalpy](#stagnation-enthalpy)
- [Enthalpy of mixing](#enthalpy-of-mixing)
- [Reaction enthalpy](#reaction-enthalpy)
- [Molar enthalpy](#molar-enthalpy)
- [Isenthalpic process](#isenthalpic-process)
- [Steady-flow energy balance](#steady-flow-energy-balance)
- [Joule-Thomson effect](#joule-thomson-effect)
  - [Measuring the Joule-Thomson effect with a porous plug](#measuring-the-joule-thomson-effect-with-a-porous-plug)
- [Joule-Thomson coefficient](#joule-thomson-coefficient)
  - [Joule-Thomson inversion curve](#joule-thomson-inversion-curve)
    - [Joule-Thomson inversion temperature](#joule-thomson-inversion-temperature)
  - [Van der Waals throttling model](#van-der-waals-throttling-model)
  - [Virial criterion for Joule-Thomson cooling](#virial-criterion-for-joule-thomson-cooling)
- [Specific enthalpy](#specific-enthalpy)
  - [Polytropic enthalpy](#polytropic-enthalpy)
- [Enthalpy Maxwell relation](#enthalpy-maxwell-relation)
- [Heat capacity at constant pressure](#heat-capacity-at-constant-pressure)
  - [Difference between constant-pressure and constant-volume heat capacities](#difference-between-constant-pressure-and-constant-volume-heat-capacities)
    - [Heat-capacity difference and mechanical stability](#heat-capacity-difference-and-mechanical-stability)
    - [Volume derivative form of the heat-capacity difference](#volume-derivative-form-of-the-heat-capacity-difference)

## Stagnation enthalpy

↑ **Parent:** [Enthalpy](enthalpy.md)

The sum of specific [enthalpy](enthalpy.md) and macroscopic [kinetic energy](energy.md#kinetic-energy) per unit [mass](classical-mechanics.md#mass). In a steady adiabatic flow without shaft work, its change is determined by the change in external [potential energy](energy.md#potential-energy). At essentially constant external [potential energy](energy.md#potential-energy), it is conserved through a stationary nonradiating [shock wave](transport-equation.md#shock-wave) even though [entropy](entropy.md) increases.

## Enthalpy of mixing

↑ **Parent:** [Enthalpy](enthalpy.md)

The mixture enthalpy minus the sum of the unmixed component enthalpies at the same [temperature](temperature.md) and pressure. Its sign does not alone determine miscibility, which depends on the full [Gibbs free energy](thermodynamic-potential.md#gibbs-free-energy).

## Reaction enthalpy

↑ **Parent:** [Enthalpy](enthalpy.md)

The [enthalpy](enthalpy.md) change per specified extent of a reaction. Scaling or reversing a [chemical equation](chemical-reaction.md#chemical-equation) scales or reverses this quantity.

## Molar enthalpy

↑ **Parent:** [Enthalpy](enthalpy.md)

[Molar enthalpy](#molar-enthalpy) is [enthalpy](enthalpy.md) per [amount of substance](physics.md#amount-of-substance) $n$, measured in $\mathrm{J\,mol^{-1}}$. With $u_{\rm m}=U/n$ and [molar volume](thermodynamics.md#molar-volume) $v_{\rm m}=V/n$, $h_{\rm m}=u_{\rm m}+pv_{\rm m}$. Its fixed-[pressure](pressure.md) [temperature](temperature.md) derivative is the corresponding [molar heat capacity](heat.md#molar-heat-capacity) $C_{p,\rm m}$, at fixed composition.

## Isenthalpic process

↑ **Parent:** [Enthalpy](enthalpy.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Isenthalpic_process)

An [isenthalpic process](#isenthalpic-process) preserves [enthalpy](enthalpy.md) for a fixed amount of material, or preserves [specific enthalpy](#specific-enthalpy) between inlet and outlet when comparing a flowing [fluid](fluid-mechanics.md#fluid) of fixed composition. It need not preserve [temperature](temperature.md) or [entropy](entropy.md). An insulated throttle satisfying the [steady-flow energy balance](#steady-flow-energy-balance) assumptions is an important example.

## Steady-flow energy balance

↑ **Parent:** [Enthalpy](enthalpy.md)

For [steady flow](fluid-mechanics.md#steady-flow) through a fixed [control volume](fluid-mechanics.md#control-volume) with one inlet and one outlet, the [first law of thermodynamics](first-law-of-thermodynamics.md) and conservation of [mass](classical-mechanics.md#mass) give

$$
\dot Q-\dot W_s=\dot m\left[h_2-h_1+\frac{w_2^2-w_1^2}{2}+g(z_2-z_1)\right].
$$

Here $\dot m$ is the [mass flow rate](fluid-mechanics.md#mass-flow-rate), $\dot Q$ incoming [heat](heat.md) per unit time, $\dot W_s$ outgoing non-flow [work](energy.md#work) per unit time, $w$ the flow speed, $z$ elevation and $g$ [gravitational acceleration](newton-s-law-of-universal-gravitation.md#gravitational-acceleration). The [specific enthalpy](#specific-enthalpy) $h=u+p/\rho$ includes both the transported [internal energy](internal-energy.md) per unit [mass](classical-mechanics.md#mass) $u$ and the [pressure](pressure.md) [work](energy.md#work) needed to push [volume](thermodynamics.md#volume-thermodynamics) through the boundary; $\rho$ is [mass density](fluid-mechanics.md#density). The inlet supplies that [pressure](pressure.md) [work](energy.md#work), while the outlet consumes it to displace the downstream [fluid](fluid-mechanics.md#fluid).[§2.5.1–2.5.2, equation 2.11: mass conservation, transported enthalpy and the steady-flow energy equation](physics-bibliography.md#thermodynamics-and-propulsion)

For an insulated stationary throttle, require negligible [heat](heat.md) transfer, no shaft or other non-flow [work](energy.md#work), and negligible changes in bulk [kinetic energy](energy.md#kinetic-energy) and gravitational [potential energy](energy.md#potential-energy). Then $h_2=h_1$. With unchanged composition this is also equality of [molar enthalpy](#molar-enthalpy). The upstream and downstream states must admit equilibrium [pressure](pressure.md), [temperature](temperature.md) and property values, although the constriction itself is irreversible and can be far from [thermodynamic equilibrium](thermodynamics.md#thermodynamic-equilibrium). Start-up storage of [energy](energy.md) in the walls and [fluid](fluid-mechanics.md#fluid), heat leakage, or a large outlet speed invalidates the reduced balance. A nozzle can convert [specific enthalpy](#specific-enthalpy) into bulk [kinetic energy](energy.md#kinetic-energy) even when it is insulated.

The same accounting for a fixed transported amount is $U_2-U_1=p_1V_1-p_2V_2$, hence $U_1+p_1V_1=U_2+p_2V_2$. This explains why dropping the two [pressure](pressure.md) [work](energy.md#work) terms would give the wrong conserved quantity.[Fitzpatrick, Joule-Thompson Throttling, equations 6.167–6.174: inlet/outlet pressure work and enthalpy conservation](physics-bibliography.md#thermodynamics-and-statistical-mechanics-by-richard-fitzpatrick/joule-thompson-throttling)

## Joule-Thomson effect

↑ **Parent:** [Enthalpy](enthalpy.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Joule–Thomson_effect)

The [Joule-Thomson effect](#joule-thomson-effect) is the [temperature](temperature.md) response of a [fluid](fluid-mechanics.md#fluid) flowing from higher to lower [pressure](pressure.md) through a valve or a plug of [porous medium](porous-media-flow.md#porous-medium), when the throttle is insulated and the other [steady-flow energy balance](#steady-flow-energy-balance) assumptions hold. Its equilibrium endpoints have equal [specific enthalpy](#specific-enthalpy). The [Joule-Thomson coefficient](#joule-thomson-coefficient) determines whether a small drop cools or warms; cooling is not universal.

<a id="joule-thomson-throttle-enthalpy-balance"></a>
![](joule-thomson-throttle-enthalpy-balance.png)

**[Figure 1](#joule-thomson-throttle-enthalpy-balance). Enthalpy accounting for an insulated Joule-Thomson effect throttle**. Original schematic of the [steady-flow energy balance](#steady-flow-energy-balance), with $u$ denoting [internal energy](internal-energy.md) per unit [mass](classical-mechanics.md#mass). The arrows include inlet and outlet [pressure](pressure.md) [work](energy.md#work). The reduced balance requires negligible bulk [kinetic energy](energy.md#kinetic-energy) and [potential energy](energy.md#potential-energy) changes. No particular apparatus or measured [temperature](temperature.md) drop is depicted.

A useful contrast is between three insulated expansions. In [free expansion](thermodynamics.md#free-expansion) of a gas-only [closed system](thermodynamics.md#closed-system) into a [vacuum](physics.md#vacuum), no external [work](energy.md#work) occurs and $U_2=U_1$; an [ideal gas](ideal-gas.md) returns to its initial equilibrium [temperature](temperature.md). In a throttle, continuous flow carries [pressure](pressure.md) [work](energy.md#work) across the boundary and preserves [specific enthalpy](#specific-enthalpy) under the stated assumptions; an [ideal gas](ideal-gas.md) again has no endpoint [temperature](temperature.md) change. In a reversible [adiabatic expansion](first-law-of-thermodynamics.md#adiabatic-expansion) of a loaded [closed system](thermodynamics.md#closed-system), the [gas](thermodynamics.md#gas) supplies [work](energy.md#work), loses [internal energy](internal-energy.md) and cools, even if it is an [ideal gas](ideal-gas.md). That process preserves [entropy](entropy.md); throttling generally produces [entropy](entropy.md). For a small constant-[enthalpy](enthalpy.md) step, $dH=T\,dS+V\,dp=0$ gives $dS=-V\,dp/T>0$ when $dp<0$ and $T,V>0$. This equilibrium comparison computes endpoint [entropy](entropy.md) differences without supplying a reversible path through the plug.

The effect is useful in [refrigerators](thermodynamics.md#refrigerator) because an appropriately prepared [real gas](thermodynamics.md#real-gas) can cool while passing through a simple valve. The inlet must lie in a suitable positive-[Joule-Thomson coefficient](#joule-thomson-coefficient) region. The [Joule-Thomson inversion curve](#joule-thomson-inversion-curve) makes that requirement precise; a pressure drop by itself is not a guarantee of refrigeration.

### Measuring the Joule-Thomson effect with a porous plug

↑ **Parent:** [Joule-Thomson effect](#joule-thomson-effect)

The 2024 operating instructions for PHYWE's 04361-00 apparatus describe a frit between two gas chambers. A copper-coil [heat exchanger](heat.md#heat-exchanger) first restores inlet [temperature](temperature.md) after cylinder-regulator cooling. An upstream manometer reads [gauge pressure](fluid-mechanics.md#gauge-pressure); the outlet stays at [atmospheric pressure](pressure.md#atmospheric-pressure). Two NiCr-Ni [thermocouples](thermoelectric-effect.md#thermocouple) sit 2–5 mm from the frit. The digital meter's difference mode reports $0.01\,\mathrm K$ precision.[PHYWE, Joule-Thomson apparatus 04361-00, 2024 instructions, pp. 1–2, sections 2–4: heat exchanger, frit, manometer, probes and difference readout](physics-bibliography.md#joule-thomson-apparatus-04361-00-operating-instructions-by-phywe)

The manual specifies at most $1\,\mathrm{bar}$ [gauge pressure](fluid-mechanics.md#gauge-pressure), one hour of apparatus acclimatization, half an hour of meter warm-up, about 1.5 minutes of flow settling, then 10–15 seconds of averaging. It identifies a stagnant-gas zeroing error that shifts the fitted intercept and notes a maximum [nitrogen](chemical-substance.md#nitrogen) signal of about $0.3\,\mathrm K$ in this setup.[PHYWE, 2024 instructions, p. 2, section 4, Hints concerning the experiment: pressure limit, equilibration, drift, averaging and zero compensation](physics-bibliography.md#joule-thomson-apparatus-04361-00-operating-instructions-by-phywe)

Define $x=p_1-p_2>0$ and $y=T_1-T_2$, so a small-drop fit is $y\simeq\mu_{\rm JT}x+c$. A constant sensor offset $c$ leaves the slope unchanged; pressure-dependent drift or [heat](heat.md) leakage can alter it. The observable is the differential [temperature](temperature.md) slope across the plug, not cylinder-outlet cooling. Display precision alone does not establish accuracy or prove an [isenthalpic process](#isenthalpic-process). This low-pressure, room-temperature apparatus does not map a complete [Joule-Thomson inversion curve](#joule-thomson-inversion-curve).

## Joule-Thomson coefficient

↑ **Parent:** [Enthalpy](enthalpy.md)

The [Joule-Thomson coefficient](#joule-thomson-coefficient) is the local [temperature](temperature.md) response to changing [pressure](pressure.md) at fixed [enthalpy](enthalpy.md) and fixed amount and composition:

$$
\mu_{\rm JT}=\left(\frac{\partial T}{\partial p}\right)_H,
\qquad [\mu_{\rm JT}]=\mathrm{K\,Pa^{-1}}.
$$

It describes the equilibrium endpoints of a [Joule-Thomson effect](#joule-thomson-effect) experiment meeting the [steady-flow energy balance](#steady-flow-energy-balance) assumptions. With $\Delta p=p_2-p_1<0$, a sufficiently small drop gives $\Delta T\simeq\mu_{\rm JT}\Delta p$. Thus $\mu_{\rm JT}>0$ means cooling, $\mu_{\rm JT}<0$ warming, and $\mu_{\rm JT}=0$ no first-order change. At zero coefficient, a finite drop can still change [temperature](temperature.md). For a chosen illustrative local value $\mu_{\rm JT}=0.20\,\mathrm{K\,bar^{-1}}$ and $\Delta p=-0.50\,\mathrm{bar}$, the linear prediction is $\Delta T=-0.10\,\mathrm K$; these are stipulated numbers, not measured gas properties.

For a fixed-composition [simple compressible system](thermodynamics.md#simple-compressible-system), the measurable form is

$$
\mu_{\rm JT}
=\frac{T(\partial V/\partial T)_p-V}{C_p}
=\frac{V}{C_p}(T\alpha-1).
$$

Here $C_p$ is the whole sample's [heat capacity at constant pressure](#heat-capacity-at-constant-pressure) and $\alpha$ its volumetric [coefficient of thermal expansion](thermodynamics.md#coefficient-of-thermal-expansion); alternatively use [molar volume](thermodynamics.md#molar-volume) and [molar heat capacity](heat.md#molar-heat-capacity) consistently. An [ideal gas](ideal-gas.md) has $\alpha=1/T$, so $\mu_{\rm JT}=0$. Its [enthalpy](enthalpy.md) depends only on [temperature](temperature.md); positive [heat capacity at constant pressure](#heat-capacity-at-constant-pressure) then makes any such finite throttle preserve [temperature](temperature.md). A [real gas](thermodynamics.md#real-gas) can have either sign. For $C_p>0$, compare $T\alpha$ with one: the [thermal expansion](thermodynamics.md#thermal-expansion) response decides the sign, not insulation alone.[Fitzpatrick, Joule-Thompson Throttling, equations 6.175–6.182: ideal-gas limit and coefficient](physics-bibliography.md#thermodynamics-and-statistical-mechanics-by-richard-fitzpatrick/joule-thompson-throttling)

A short derivation uses $dH=T\,dS+V\,dp$ and the [Maxwell relation](thermodynamics.md#maxwell-relations) $(\partial S/\partial p)_T=-(\partial V/\partial T)_p$:

$$
dH=C_p\,dT+\left[V-T\left(\frac{\partial V}{\partial T}\right)_p\right]dp.
$$

Setting $dH=0$ gives the coefficient. These are equilibrium [state function](thermodynamics.md#state-function) identities, not a claim of a [reversible thermodynamic process](second-law-of-thermodynamics.md#reversible-thermodynamic-process) inside the throttle. For a finite drop, solve the endpoint [enthalpy](enthalpy.md) equality or integrate

$$
T_2-T_1=\int_{p_1}^{p_2}\mu_{\rm JT}(T(p),p)\,dp
$$

along the constant-[enthalpy](enthalpy.md) equilibrium curve. The coefficient can change sign during that integration, as the [Van der Waals throttling model](#van-der-waals-throttling-model) illustrates.

### Joule-Thomson inversion curve

↑ **Parent:** [Joule-Thomson coefficient](#joule-thomson-coefficient)

The [Joule-Thomson inversion curve](#joule-thomson-inversion-curve) is the set of equilibrium [temperature](temperature.md)–[pressure](pressure.md) states where the [Joule-Thomson coefficient](#joule-thomson-coefficient) vanishes. For positive [heat capacity at constant pressure](#heat-capacity-at-constant-pressure), its condition is $T\alpha=1$, with $\alpha$ the [coefficient of thermal expansion](thermodynamics.md#coefficient-of-thermal-expansion). The curve separates locally cooling and warming throttle regions. A finite [isenthalpic process](#isenthalpic-process) can cross it, so the inlet sign alone does not fix the total [temperature](temperature.md) change. An [ideal gas](ideal-gas.md) has zero coefficient everywhere, rather than an isolated dividing curve.

#### Joule-Thomson inversion temperature

↑ **Parent:** [Joule-Thomson inversion curve](#joule-thomson-inversion-curve)

A [Joule-Thomson inversion temperature](#joule-thomson-inversion-temperature) is a [temperature](temperature.md) at which the [Joule-Thomson coefficient](#joule-thomson-coefficient) is zero at a specified [pressure](pressure.md). There can be more than one such [temperature](temperature.md) at that [pressure](pressure.md); distinguish the upper and lower branches from a maximum or a dilute-gas limiting value.

### Van der Waals throttling model

↑ **Parent:** [Joule-Thomson coefficient](#joule-thomson-coefficient)

A hypothetical [Van der Waals equation](pressure.md#van-der-waals-equation) model illustrates positive and negative [Joule-Thomson coefficient](#joule-thomson-coefficient) regions and a finite throttle that first warms, then cools. Use the molar convention already distinguished in [Van der Waals equation](pressure.md#van-der-waals-equation):

$$
p=\frac{RT}{v_{\rm m}-b_{\rm m}}-\frac{a_{\rm m}}{v_{\rm m}^2},
\qquad
u_{\rm m}=C_{V,\rm m}T-\frac{a_{\rm m}}{v_{\rm m}},
\qquad C_{V,\rm m}=\frac32R.
$$

Here $v_{\rm m}$ is [molar volume](thermodynamics.md#molar-volume), $R$ the [molar gas constant](ideal-gas.md#molar-gas-constant), $u_{\rm m}$ [internal energy](internal-energy.md) per [mole](physics.md#mole-unit), and $C_{V,\rm m}$ the stipulated constant [molar heat capacity](heat.md#molar-heat-capacity) at fixed [volume](thermodynamics.md#volume-thermodynamics). The second equation is an additional caloric assumption: an [equation of state](pressure.md#equation-of-state) alone does not specify the [temperature](temperature.md) dependence of [internal energy](internal-energy.md). It satisfies the equilibrium identity $(\partial u_{\rm m}/\partial v_{\rm m})_T=T(\partial p/\partial T)_{v_{\rm m}}-p=a_{\rm m}/v_{\rm m}^2$. The arbitrary [energy](energy.md) reference is set to zero.

<a id="van-der-waals-throttling-inversion-model"></a>
![](van-der-waals-throttling-inversion-model.png)

**[Figure 2](#van-der-waals-throttling-inversion-model). Hypothetical Van der Waals throttling model: Joule-Thomson inversion curve and finite temperature responses**. All curves are original model calculations, not [nitrogen](chemical-substance.md#nitrogen), [carbon dioxide](chemical-substance.md#carbon-dioxide) or other gas measurements. Colors label the response along constant [molar enthalpy](#molar-enthalpy); arrows point toward lower [pressure](pressure.md). The displayed states are above the model [Van der Waals critical point](pressure.md#van-der-waals-critical-point) [temperature](temperature.md) and have positive [isothermal compressibility](thermodynamics.md#isothermal-compressibility). The purple path crosses the zero-coefficient curve and has a [temperature](temperature.md) maximum.

Define dimensionless variables $r=v_{\rm m}/b_{\rm m}$, $\theta=Rb_{\rm m}T/a_{\rm m}$, $\pi=b_{\rm m}^2p/a_{\rm m}$ and $\eta=b_{\rm m}h_{\rm m}/a_{\rm m}$, where $h_{\rm m}$ is [molar enthalpy](#molar-enthalpy). These differ from the critical-value scaling in [Van der Waals law of corresponding states](pressure.md#van-der-waals-law-of-corresponding-states). The throttle calculation reduces to

$$
\pi=\frac{\theta}{r-1}-\frac1{r^2},\qquad
\eta=\frac32\theta+\pi r-\frac1r,
\qquad
\theta(r;\eta)=\frac{\eta+2/r}{3/2+r/(r-1)}.
$$

Thus a prescribed inlet fixes $\eta$, and solving the first and last equations at the outlet [pressure](pressure.md) gives the final [temperature](temperature.md). For an inlet $(\theta_1,\pi_1)=(0.8,0.12)$ and outlet $\pi_2=0.025$, the model gives $\theta_2\simeq0.752287$, a decrease of $0.047713$. The inlet $(2.2,0.12)$ instead gives $\theta_2\simeq2.205786$, an increase of $0.005786$. The purple inlet $(1.45,0.30)$ initially warms but ends at $\theta_2\simeq1.437585$ for the same outlet [pressure](pressure.md). These are reduced toy values, not kelvin readings or experimental evidence. No physical gas parameters were fitted.

For a short inversion derivation, implicit [differentiation](calculus.md#differentiation) of the [Van der Waals equation](pressure.md#van-der-waals-equation) at fixed [pressure](pressure.md) gives

$$
\left(\frac{\partial v_{\rm m}}{\partial T}\right)_p
=\frac{R/(v_{\rm m}-b_{\rm m})}{RT/(v_{\rm m}-b_{\rm m})^2-2a_{\rm m}/v_{\rm m}^3}.
$$

Insert this into $T(\partial v_{\rm m}/\partial T)_p=v_{\rm m}$ and substitute back into the [equation of state](pressure.md#equation-of-state). The [Joule-Thomson inversion curve](#joule-thomson-inversion-curve) is

$$
T_{\rm inv}=\frac{2a_{\rm m}}{Rb_{\rm m}}\left(1-\frac{b_{\rm m}}{v_{\rm m}}\right)^2,
\qquad
\theta_{\rm inv}=2(1-1/r)^2,
\qquad
\pi_{\rm inv}=\frac{2r-3}{r^2}.
$$

Positive inversion [pressure](pressure.md) requires $r>3/2$. Its maximum [pressure](pressure.md) is $\pi=1/3$ at $r=3$, while the upper dilute limit is $\theta_{\rm inv}\to2$. Using [Van der Waals critical point](pressure.md#van-der-waals-critical-point) values, the latter is $T_{\rm inv,max}/T_c=27/4$. The inversion locus depends on the [equation of state](pressure.md#equation-of-state); the chosen [molar heat capacity](heat.md#molar-heat-capacity) additionally determines how much [temperature](temperature.md) changes along each finite throttle.[Fitzpatrick, Joule-Thompson Throttling, equations 6.188–6.190 and following paragraph: inversion locus, maximum temperature and limits of the van der Waals prediction](physics-bibliography.md#thermodynamics-and-statistical-mechanics-by-richard-fitzpatrick/joule-thompson-throttling)

The displayed region has $\theta>8/27$, above the model's critical [temperature](temperature.md), and uses only $r>1$, $p>0$, $(\partial p/\partial v_{\rm m})_T<0$ and positive $C_{p,\rm m}$. Subcritical calculations require attention to [phase coexistence](critical-phenomenon.md#phase-coexistence), [metastability](critical-phenomenon.md#metastability) and the [Maxwell construction](thermodynamic-potential.md#maxwell-construction); an unstable homogeneous continuation is not an equilibrium throttle endpoint. Even on a stable branch, this [mean-field theory](statistical-physics.md#mean-field-theory) with constant $C_{V,\rm m}$ is a qualitative model, not an accurate inversion map for a particular [real gas](thermodynamics.md#real-gas). [Phase transitions](critical-phenomenon.md#phase-transition), changing composition, appreciable [heat](heat.md) leakage or bulk [kinetic energy](energy.md#kinetic-energy) changes require a different property calculation or [steady-flow energy balance](#steady-flow-energy-balance). At [phase coexistence](critical-phenomenon.md#phase-coexistence), the smooth single-[thermodynamic phase](thermodynamics.md#thermodynamic-phase) coefficient formula cannot replace a balance involving the [phase fraction](thermodynamics.md#phase-fraction).

### Virial criterion for Joule-Thomson cooling

↑ **Parent:** [Joule-Thomson coefficient](#joule-thomson-coefficient)

For $p=k_BT[n+B_2(T)n^2]$, the coefficient is $\mu=N[TB_2'-B_2]/[C_p(1+2B_2n)]$. On the stable dilute branch it is positive precisely when $d(B_2/T)/dT>0$.

## Specific enthalpy

↑ **Parent:** [Enthalpy](enthalpy.md)

Specific enthalpy is [enthalpy](enthalpy.md) per unit mass. For a simple compressible fluid of fixed composition, the [first law of thermodynamics](first-law-of-thermodynamics.md) gives

$$
dh=T\,ds+\frac{dp}{\rho},
$$

where $T$ is [temperature](temperature.md), $s$ is [specific entropy](entropy.md#specific-entropy), $p$ is [pressure](pressure.md), and $\rho$ is [mass density](fluid-mechanics.md#density). Along an [isentropic flow](compressible-flow.md#isentropic-flow), $dh=dp/\rho$. For a [perfect gas](ideal-gas.md) with constant [specific-heat ratio](ideal-gas.md#heat-capacity-ratio) $\gamma$, $h=\gamma p/[(\gamma-1)\rho]$.

### Polytropic enthalpy

↑ **Parent:** [Specific enthalpy](#specific-enthalpy)

For $p=K\rho^{1+1/n}$ with $K,n>0$, the specific [enthalpy](enthalpy.md) relative to vacuum is $Q=(n+1)K\rho^{1/n}=(n+1)p/\rho$. It obeys $\nabla Q=\nabla p/\rho$ and $nD_tQ=-Q\nabla\cdot\mathbf u$. The vacuum reference is fixed when these equations are combined with the [polytropic equation of state](astrophysical-fluid-dynamics.md#polytropic-equation-of-state).

## Enthalpy Maxwell relation

↑ **Parent:** [Enthalpy](enthalpy.md)

Since $T=(\partial H/\partial S)_p$ and $V=(\partial H/\partial p)_S$, equality of mixed derivatives gives $(\partial T/\partial p)_S=(\partial V/\partial S)_p$.

## Heat capacity at constant pressure

↑ **Parent:** [Enthalpy](enthalpy.md)

For a fixed-composition [closed system](thermodynamics.md#closed-system), the [heat capacity](heat.md#heat-capacity) at fixed [pressure](pressure.md) is $C_p=(\partial H/\partial T)_p$, with [enthalpy](enthalpy.md) $H$. Under the [quasistatic process](thermodynamics.md#quasistatic-process) assumptions in [heat capacity](heat.md#heat-capacity), only [pressure](pressure.md)-[volume](thermodynamics.md#volume-thermodynamics) [work](energy.md#work) is permitted, so $dp=0$ gives $\delta Q=dH=C_p\,dT$. Thus supplied [heat](heat.md) is $Q=\Delta H$, or $Q=C_p\Delta T$ within a single [thermodynamic phase](thermodynamics.md#thermodynamic-phase) when $C_p$ is constant. For an [ideal gas](ideal-gas.md), the expansion [work](energy.md#work) explains why this exceeds the required [heat](heat.md) at fixed [volume](thermodynamics.md#volume-thermodynamics) for the same [temperature](temperature.md) increase. Its per-unit-[mass](classical-mechanics.md#mass) counterpart is [specific heat capacity at constant pressure](heat.md#specific-heat-capacity-at-constant-pressure).

### Difference between constant-pressure and constant-volume heat capacities

↑ **Parent:** [Heat capacity at constant pressure](#heat-capacity-at-constant-pressure)

For a simple compressible system,

$$
C_P-C_V
=T\left(\frac{\partial V}{\partial T}\right)_P
\left(\frac{\partial P}{\partial T}\right)_V.
$$

This follows by expressing the entropy as a function of temperature and volume and using a Maxwell relation.

#### Heat-capacity difference and mechanical stability

↑ **Parent:** [Difference between constant-pressure and constant-volume heat capacities](#difference-between-constant-pressure-and-constant-volume-heat-capacities)

For a fixed-composition [simple compressible system](thermodynamics.md#simple-compressible-system), a [Maxwell relation](thermodynamics.md#maxwell-relations) gives $C_p-C_V=T(\partial p/\partial T)_V(\partial V/\partial T)_p$. At fixed [volume](geometry-and-topology.md#volume), the differential [equation of state](pressure.md#equation-of-state) gives $(\partial p/\partial T)_V=\alpha_V/\kappa_T$, proving the displayed result. Positive absolute [temperature](temperature.md) and positive [isothermal compressibility](thermodynamics.md#isothermal-compressibility) imply a nonnegative difference. It vanishes when [thermal expansion](thermodynamics.md#thermal-expansion) does, so strict inequality requires a nonzero expansion coefficient. This stability argument includes nonideal internal-energy changes, unlike a purely ideal-gas expansion-work explanation.

#### Volume derivative form of the heat-capacity difference

↑ **Parent:** [Difference between constant-pressure and constant-volume heat capacities](#difference-between-constant-pressure-and-constant-volume-heat-capacities)

For a fixed-composition simple compressible [thermodynamic system](thermodynamics.md#thermodynamic-system) with smooth [equations of state](pressure.md#equation-of-state), write the [internal energy](internal-energy.md) as $U(T,V)$ and the [enthalpy](enthalpy.md) as $H=U+pV$. Differentiating $H$ at constant [pressure](pressure.md) and applying the [multivariable chain rule](calculus.md#multivariable-chain-rule) gives

$$
C_p=\left(\frac{\partial U}{\partial T}\right)_p+p\left(\frac{\partial V}{\partial T}\right)_p,\qquad\left(\frac{\partial U}{\partial T}\right)_p=\left(\frac{\partial U}{\partial T}\right)_V+\left(\frac{\partial U}{\partial V}\right)_T\left(\frac{\partial V}{\partial T}\right)_p.
$$

Subtracting the [heat capacity at constant volume](heat.md#heat-capacity-at-constant-volume) proves the displayed identity. For an [ideal gas](ideal-gas.md), $(\partial U/\partial V)_T=0$ and $(\partial V/\partial T)_p=Nk_B/p$, so $C_p-C_V=Nk_B$. For a nonideal material the [internal energy](internal-energy.md) change with [volume](thermodynamics.md#volume-thermodynamics) contributes as well as expansion [work](energy.md#work).

## ↑ Ancestors (5)

1. [Thermodynamics](thermodynamics.md)
2. [Statistical physics](statistical-physics.md)
3. [Branches of physics](physics.md#branches-of-physics)
4. [Physics](physics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (126)

- [Activation energy](chemical-kinetics.md#activation-energy)
- [Advection-driven melting front in a porous matrix](geophysics.md#advection-driven-melting-front-in-a-porous-matrix)
- [Bond-dissociation energy](chemical-bond.md#bond-dissociation-energy)
- [Bond-dissociation enthalpy](chemical-bond.md#bond-dissociation-enthalpy)
- [Born-Haber cycle](ionic-bonding.md#born-haber-cycle)
- [Calorimeter calibration](calorimetry.md#calorimeter-calibration)
- [Calorimetry](calorimetry.md)
- [Clausius-Clapeyron relation](thermodynamic-potential.md#clausius-clapeyron-relation)
- [Desolvation](ionic-bonding.md#desolvation)
- [Electrical calorimetry of a resistor](electric-charge.md#electrical-calorimetry-of-a-resistor)
- [Electron attachment enthalpy](electronegativity.md#electron-attachment-enthalpy)
- [Energy profile (chemistry)](chemical-kinetics.md#energy-profile-chemistry)
- [Enthalpy](enthalpy.md)
- [Enthalpy change of solution](chemistry.md#enthalpy-change-of-solution)
- [Enthalpy cycle](chemistry.md#enthalpy-cycle)
- [Enthalpy of activation](chemical-kinetics.md#enthalpy-of-activation)
- [Enthalpy of atomization](chemistry.md#enthalpy-of-atomization)
- [Enthalpy of vaporization](critical-phenomenon.md#enthalpy-of-vaporization)
- [Entropy generation by mixing equal thermal masses](second-law-of-thermodynamics.md#entropy-generation-by-mixing-equal-thermal-masses)
- [Frazil export enthalpy balance](geophysics.md#frazil-export-enthalpy-balance)
- [Free expansion](thermodynamics.md#free-expansion)
- [Gibbs free energy](thermodynamic-potential.md#gibbs-free-energy)
- [Gibbs free energy of mixing](mixture.md#gibbs-free-energy-of-mixing)
- [Heat](heat.md)
- [Heat capacity](heat.md#heat-capacity)
- [Heat capacity at constant pressure](#heat-capacity-at-constant-pressure)
- [Helium liquefaction](temperature.md#helium-liquefaction)
- [Hess's law](chemistry.md#hess-s-law)
- [Hess's law calorimetry experiment](chemistry.md#hess-s-law-calorimetry-experiment)
- [Hess's law equation cancellation](chemistry.md#hess-s-law-equation-cancellation)
- [Hydration enthalpy](ionic-bonding.md#hydration-enthalpy)
- [Hydrophobic effect](physical-chemistry.md#hydrophobic-effect)
- [Ice-melting calorimetry](statistical-physics.md#ice-melting-calorimetry)
- [Internal energy at constant temperature](internal-energy.md#internal-energy-at-constant-temperature)
- [Isenthalpic process](#isenthalpic-process)
- [James Prescott Joule](physicist.md#james-prescott-joule)
- [Joule-Thomson coefficient](#joule-thomson-coefficient)
- [Joule-Thomson effect](#joule-thomson-effect)
- [Kirchhoff's law of thermochemistry](chemistry.md#kirchhoff-s-law-of-thermochemistry)
- [Latent heat](thermodynamic-potential.md#latent-heat)
- [Latent heat of fusion](statistical-physics.md#latent-heat-of-fusion)
- [Lattice energy](ionic-bonding.md#lattice-energy)
- [Lattice enthalpy from solution calorimetry](ionic-bonding.md#lattice-enthalpy-from-solution-calorimetry)
- [Liquefaction enthalpy budget](temperature.md#liquefaction-enthalpy-budget)
- [Maxwell relations](thermodynamics.md#maxwell-relations)
- [Mayer's relation](ideal-gas.md#mayer-s-relation)
- [Melting-front instability due to permeability contrast](porous-media-flow.md#melting-front-instability-due-to-permeability-contrast)
- [Melting pressure inferred from flotation and latent heats](thermodynamic-potential.md#melting-pressure-inferred-from-flotation-and-latent-heats)
- [Mixing calorimetry](calorimetry.md#mixing-calorimetry)
- [Molar enthalpy](#molar-enthalpy)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2012/paper-1.md#2/a/solution)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2012/paper-1.md#2/c/solution)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2017.md#3/b/solution)
- [Solution](past-exam-of-the-chemistry-b-course-of-the-university-of-cambridge/2022/paper-1.md#b5/a/iii/solution)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1.md#4/a/iii/solution)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1.md#4/a/vi/solution)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1.md#4/b/i/solution)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1.md#4/b/ii/solution)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1.md#5/c/iii/solution)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1.md#6/a/iii/solution)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1.md#6/a/iv/solution)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-1.md#2/a/v/solution)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-1.md#4/a/solution)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-1.md#4/b/solution)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-1.md#5/c/v/solution)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1.md#10/b/ii/solution)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1.md#10/b/iii/solution)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-3.md#47/a/solution)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-3.md#47/b/solution)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-3.md#47/c/solution)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-id.md#2/a/solution)
- [Solution](past-exam-of-the-formation-of-structure-in-the-universe-course-of-the-university-of-cambridge/2012/paper-1.md#1/c/solution)
- [Solution](past-exam-of-the-formation-of-structure-in-the-universe-course-of-the-university-of-cambridge/2014/paper-1.md#3/a/solution)
- [Solution](past-exam-of-the-materials-science-course-of-the-university-of-cambridge/2015/paper-1.md#4/a/solution)
- [Solution](past-exam-of-the-materials-science-course-of-the-university-of-cambridge/2016/paper-1.md#6/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-35.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-77.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-4.md#34d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-70.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-71.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-2.md#34d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-65.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-65.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-89.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-3.md#35c/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-80.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-3.md#33c/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-315.md#2/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-314.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-332.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-332.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ii/paper-2.md#37c/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-4.md#39c/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-314.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2003/paper-2.md#9/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-2.md#17/a/solution)
- [Solution](past-exam-of-the-mphil-in-micro-and-nanotechnology-enterprise-course-of-the-university-of-cambridge/2017/paper-1.md#section-a-iii/6/ii/solution)
- [Solution](past-exam-of-the-mphil-in-micro-and-nanotechnology-enterprise-course-of-the-university-of-cambridge/2021/paper-1.md#10/i/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2011/paper-1.md#section-c/c10/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2012/paper-2.md#section-c/c10/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2012/paper-2.md#section-c/c13/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2013/paper-2.md#section-c/c11/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2017/paper-2.md#section-c/c11/b/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2018/paper-2.md#section-c/c13/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2022/paper-2.md#section-a/a4/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2022/paper-2.md#section-c/c8/e/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-1.md#section-b/b3/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-1.md#b1/solution)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2004.md#section-b/b7/a/solution)
- [Solution](past-exam-of-the-relativistic-astrophysics-and-cosmology-course-of-the-university-of-cambridge/2013/paper-1.md#3/d/solution)
- [Solution](past-exam-of-the-relativistic-astrophysics-and-cosmology-course-of-the-university-of-cambridge/2014/paper-1.md#3/c/solution)
- [Phase diagram](thermodynamic-potential.md#phase-diagram)
- [Physical properties of salts](ionic-bonding.md#physical-properties-of-salts)
- [Polytropic enthalpy](#polytropic-enthalpy)
- [Reaction enthalpy](#reaction-enthalpy)
- [Sensible heat](heat.md#sensible-heat)
- [Sequential bond-dissociation energies](chemical-bond.md#sequential-bond-dissociation-energies)
- [Solubility](ionic-bonding.md#solubility)
- [Solvation thermodynamic balance](ionic-bonding.md#solvation-thermodynamic-balance)
- [Specific enthalpy](#specific-enthalpy)
- [Stagnation enthalpy](#stagnation-enthalpy)
- [Standard enthalpy of formation](chemistry.md#standard-enthalpy-of-formation)
- [State function](thermodynamics.md#state-function)
- [Thermodynamic potential](thermodynamic-potential.md)
- [Two reversible ideal-gas paths between the same states](thermodynamics.md#two-reversible-ideal-gas-paths-between-the-same-states)
- [Volume derivative form of the heat-capacity difference](#volume-derivative-form-of-the-heat-capacity-difference)
