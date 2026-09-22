# Paddle-wheel calorimetry energy balance

↑ **Parent:** [Joule's paddle-wheel experiment](joule-s-paddle-wheel-experiment.md)

Choose the [water](water.md), vessel and immersed paddle as the [closed system](closed-system.md), with fixed outer [volume](volume-thermodynamics.md) and negligible endpoint changes in bulk mechanical [energy](energy-split.md). Between common equilibrium [temperatures](temperature-split.md) $T_1$ and $T_2$,

$$
\Delta U_{\rm assembly}=\int_{T_1}^{T_2}C_{\rm eff}(T)\,dT
=W_{\rm shaft,on}+Q_{\rm room,in}.
$$

The effective [heat capacity](heat-capacity.md) $C_{\rm eff}$ includes every component that participates in the common [temperature](temperature-split.md) change. For nearly constant $C_{\rm eff}$, the readout is $C_{\rm eff}\Delta T$. [Heat](heat-split.md) transferred between [water](water.md) and paddle stays inside this boundary; it must not be added again as external input. The drive supplies shaft [work](work.md) even though the vessel has no expansion [work](work.md).

For a simplified modern model, let $M$ be the total descending [mass](mass.md), let each of $N$ descents cover height $h$, and let $W_{\rm loss,out}$ be [energy](energy-split.md) diverted by the external drive. With negligible remaining drive [kinetic energy](kinetic-energy.md) and elastic storage,

$$
W_{\rm shaft,on}=NMgh-W_{\rm loss,out},\qquad
NMgh=C_{\rm eff}\Delta T+W_{\rm loss,out}+Q_{\rm room,out}.
$$

The signed $Q_{\rm room,out}=-Q_{\rm room,in}$ may be negative if the room warms the assembly. This model omits the small endpoint and elastic corrections explicitly considered in the historical analysis. It does not equate all of the weights' lost [gravitational potential energy](gravitational-energy.md) with the [water](water.md)'s gained [internal energy](internal-energy-split.md).

As a proposed modern protocol, measure the falling [masses](mass.md) and distances, calibrate the [thermometer](thermometer.md) and $C_{\rm eff}$ independently, record room [temperature](temperature-split.md) and resting drift before and after each run, and wait for fluid motion to decay before the final equilibrium reading. Repeat with different fall budgets and run durations. A stable ratio of corrected input to corrected thermal storage supports the [first law of thermodynamics](first-law-of-thermodynamics-split.md) over the tested range. Resting controls only estimate leakage if their thermal conditions represent the driven run; sensor lag, nonuniform [temperature](temperature-split.md), unmeasured drive losses, evaporation or changing [heat capacity](heat-capacity.md) can spoil the inference. Those are limits of the measurement, rather than evidence that [heat](heat-split.md) was stored as a separate substance.

## ↑ Ancestors (7)

1. [Joule's paddle-wheel experiment](joule-s-paddle-wheel-experiment.md)
2. [Internal energy](internal-energy-split.md)
3. [Thermodynamics](thermodynamics-split.md)
4. [Statistical physics](statistical-physics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)
