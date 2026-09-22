# Heat engine

↑ **Parent:** [Thermodynamics](thermodynamics-split.md)

A heat engine uses a repeating [thermodynamic cycle](thermodynamic-cycle.md) to turn part of an incoming [heat](heat.md) transfer into net outgoing [work](work.md). In the two-[thermal reservoir](heat-bath.md) model, the hot [thermal reservoir](heat-bath.md) supplies [heat](heat.md) $Q_h>0$ at fixed [temperature](temperature.md) $T_h$, and the cold [thermal reservoir](heat-bath.md) receives [heat](heat.md) of magnitude $Q_c>0$ at fixed [temperature](temperature.md) $T_c<T_h$. A [Stirling engine](stirling-engine.md) makes the repeated motion visible; the abstract [energy](energy.md) budget applies independently of its particular mechanism.[§3.2, Figure 3.3: two reservoirs and net work output](thermodynamics-and-propulsion/3-2-generalized-representation-of-thermodynamic-cycles.md)

Choose the entire cyclic device as a [closed system](closed-system.md), with no net change in bulk [kinetic energy](kinetic-energy.md) or [potential energy](potential-energy.md). Count [heat](heat.md) entering as positive and net [work](work.md) delivered as positive, as in the [first law of thermodynamics](first-law-of-thermodynamics.md). Thus $Q_h$ enters with a plus sign and $Q_c$, although a positive magnitude, enters with a minus sign. Assume these two [heat](heat.md) transfers and the net [work](work.md) are the only transfers across the boundary. Over one complete [thermodynamic cycle](thermodynamic-cycle.md), all stored [energy](energy.md), including [internal energy](internal-energy.md) $U$, returns to its starting value:

$$
\Delta U=Q_h-Q_c-W=0,\qquad W=Q_h-Q_c.
$$

The device does not accumulate [heat](heat.md) from cycle to cycle. More precisely, [heat](heat.md) is a transfer, while [internal energy](internal-energy.md) is what can be stored; even a component that temporarily stores [internal energy](internal-energy.md) must return to its initial state for this boundary to be cyclic.[§3.2: heat, work and changes in stored internal energy](university-physics-volume-2-by-samuel-j-ling-and-others/3-2-work-heat-and-internal-energy.md)

For engine operation, $Q_h>Q_c$ and $W>0$. Its [thermal efficiency](thermal-efficiency.md) is

$$
\eta=\frac{W}{Q_h}=1-\frac{Q_c}{Q_h}.
$$

Use net [work](work.md), after subtracting any [work](work.md) supplied during compression or required by auxiliaries included in the chosen device. For periodic operation, average [power](power.md) satisfies $P_{\rm out}=\dot Q_h-\dot Q_c$ and $\eta=P_{\rm out}/\dot Q_h$, with the rates averaged over complete [thermodynamic cycles](thermodynamic-cycle.md).[§4.2, equations 4.1–4.2: heat-engine balance and efficiency](university-physics-volume-2-by-samuel-j-ling-and-others/4-2-heat-engines.md)

For a stipulated model at $T_h=600\,\mathrm K$ and $T_c=300\,\mathrm K$, let $Q_h=1000\,\mathrm J$ and $Q_c=600\,\mathrm J$ per [thermodynamic cycle](thermodynamic-cycle.md). Then $W=400\,\mathrm J$ and $\eta=2/5=40\%$. At two [thermodynamic cycles](thermodynamic-cycle.md) per second, these become $2000\,\mathrm W$ incoming [heat transfer](heat-transfer.md), $1200\,\mathrm W$ outgoing [heat transfer](heat-transfer.md), and $800\,\mathrm W$ net [power](power.md). These are constructed values, not measurements.

<a id="image-two-thermal-reservoir-heat-engine-1000-mathrm-j-in-400-mathrm-j-of-net-work-and-600-mathrm-j-rejected"></a>
![](heat-engine-cyclic-energy-flows.png)

**[Figure 3](#image-two-thermal-reservoir-heat-engine-1000-mathrm-j-in-400-mathrm-j-of-net-work-and-600-mathrm-j-rejected). Two-thermal reservoir heat engine: $1000\,\mathrm J$ in, $400\,\mathrm J$ of net work, and $600\,\mathrm J$ rejected**. Illustrative transfers per complete [thermodynamic cycle](thermodynamic-cycle.md), with positive magnitudes labeled on the arrows. The [closed system](closed-system.md) returns to its initial state. Arrow widths represent the [energy](energy.md) split; the [thermal reservoirs](heat-bath.md) remain at $600\,\mathrm K$ and $300\,\mathrm K$.

Different signs describe different tasks. With the same directions of [heat transfer](heat-transfer.md), $Q_h=Q_c$ gives $W=0$: a device transmitting [heat](heat.md) without net [work](work.md) output. If $Q_c>Q_h$, net [work](work.md) is supplied to that device. A [refrigerator](refrigerator.md) or [heat pump](heat-pump.md) instead extracts [heat](heat.md) from the cold side and delivers [heat](heat.md) to the hot side, using positive input [work](work.md) $W_{\rm in}$ and the balance $Q_h=Q_c+W_{\rm in}$. Their useful output is [heat transfer](heat-transfer.md), measured by a [coefficient of performance](coefficient-of-performance.md). Finally, a one-time [isothermal expansion](isothermal-expansion.md) can have $Q=W$ and $\Delta U=0$ while leaving the [volume](volume-thermodynamics.md) changed: it is not a complete [thermodynamic cycle](thermodynamic-cycle.md). A warming device also fails the cyclic assumption, and a fuel-consuming device requires an accounting of matter crossing its boundary.

For two fixed [thermal reservoirs](heat-bath.md) at positive [thermodynamic temperatures](thermodynamic-temperature.md), the [Second law of thermodynamics](second-law-of-thermodynamics.md) strengthens the [energy](energy.md) balance to

$$
\eta\le\eta_C=1-\frac{T_c}{T_h}.
$$

Equality requires the overall operation to be a [reversible thermodynamic process](reversible-thermodynamic-process.md), including its [heat transfer](heat-transfer.md) to the [thermal reservoirs](heat-bath.md). The [Carnot cycle](carnot-cycle.md) explains how the reversible benchmark is constructed, and [Carnot's theorem](carnot-s-theorem.md) explains its universality and the [entropy production](entropy-production.md) penalty. Use [kelvin](kelvin.md) values, never ratios of [degree Celsius](degree-celsius.md) readings. The example above lies below the $50\%$ bound: its total [entropy production](entropy-production.md) is $-1000/600+600/300=1/3\,\mathrm{J\,K^{-1}}$ per [thermodynamic cycle](thermodynamic-cycle.md).

<a id="image-thermal-efficiency-versus-hot-thermal-reservoir-temperature-at-t-c-300-mathrm-k"></a>
![](heat-engine-efficiency-temperature-model.png)

**[Figure 4](#image-thermal-efficiency-versus-hot-thermal-reservoir-temperature-at-t-c-300-mathrm-k). Thermal efficiency versus hot thermal reservoir temperature at $T_c=300\,\mathrm K$**. The upper curve is the reversible bound in [Carnot's theorem](carnot-s-theorem.md). The lower curve is the stipulated model $\eta=0.8\eta_C$, not experimental data or a universal engine law. At $T_h=600\,\mathrm K$, the curves give $50\%$ and $40\%$, matching the [energy](energy.md) budget above. The endpoint $T_h=T_c$ is a zero-output limit.

This is useful before building a machine: warmer cooling surroundings reduce the possible [thermal efficiency](thermal-efficiency.md), even if the mechanism is unchanged. A small observed [thermal efficiency](thermal-efficiency.md) does not by itself test the [Second law of thermodynamics](second-law-of-thermodynamics.md); [heat](heat.md) leaks, [friction](friction.md), incomplete recovery of [work](work.md), and the measurement boundary can all reduce the reported ratio. A meaningful comparison requires the actual [thermal reservoir](heat-bath.md) [temperatures](temperature.md), matched [heat](heat.md) and net [work](work.md) measurements, and the hypotheses of [Carnot's theorem](carnot-s-theorem.md). Finite bodies whose [temperatures](temperature.md) change are treated separately there.

The practical question already appears in the 1824 [Réflexions sur la puissance motrice du feu et sur les machines propres à développer cette puissance by Sadi Carnot](reflexions-sur-la-puissance-motrice-du-feu-et-sur-les-machines-propres-a-developper-cette-puissance-by-sadi-carnot.md): pp. 6–8 ask whether machines driven by [heat](heat.md) have a fundamental limit and whether changing the working substance can improve their output. Pages 9–11 describe heating and cooling in real machines, but use the historical [caloric theory](caloric-theory.md), rather than the modern [first law of thermodynamics](first-law-of-thermodynamics.md) balance. The historical discussion under [Carnot's theorem](carnot-s-theorem.md) explains that distinction.

**Table of contents**

- [Stirling engine](stirling-engine.md)
  - [Prony brake](prony-brake.md)
- [Heat-engine calorimetry](heat-engine-calorimetry.md)

## ↑ Ancestors (5)

1. [Thermodynamics](thermodynamics-split.md)
2. [Statistical physics](statistical-physics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (10)

- [Caloric theory](caloric-theory.md)
- [Carnot's theorem](carnot-s-theorem.md)
- [Clausius statement of the second law](clausius-statement-of-the-second-law.md)
- [Coefficient of performance](coefficient-of-performance.md)
- [Heat](heat.md)
- [Heat engine](heat-engine.md)
- [Ideal gas law](ideal-gas-law.md)
- [Kelvin-Planck statement of the second law](kelvin-planck-statement-of-the-second-law.md)
- [Stirling engine](stirling-engine.md)
- [Thermodynamics](thermodynamics-split.md)
