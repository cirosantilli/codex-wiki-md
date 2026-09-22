# Heat bath relaxation with finite capacity

↑ **Parent:** [Finite heat bath](finite-heat-bath.md)

The equilibrium calculation determines where the two [temperatures](temperature-split.md) end, without determining how long they take. Stipulate a constant [thermal conductance](thermal-conductance.md) $G>0$ and the linear [heat transfer](heat-transfer.md) law underlying [Newton's law of cooling](newton-s-law-of-cooling.md). With $Q$ positive from body 1 to bath 2, the [ordinary differential equations](ordinary-differential-equation.md) are

$$
\dot Q=G(T_1-T_2),\qquad C_1\dot T_1=-G(T_1-T_2),\qquad C_2\dot T_2=G(T_1-T_2).
$$

The dot denotes a [derivative](derivative.md) with respect to time. This model assumes internal equilibration is fast compared with exchange between the bodies. Adding the two [energy](energy-split.md) rates gives zero; subtracting the [temperature](temperature-split.md) rates gives

$$
\frac{d}{dt}(T_1-T_2)=-G\left(\frac1{C_1}+\frac1{C_2}\right)(T_1-T_2),\qquad
\tau=\frac{C_1C_2}{G(C_1+C_2)}.
$$

The [temperature](temperature-split.md) difference has [exponential decay](exponential-decay.md) with [time constant](time-constant.md) $\tau$. For the [finite heat bath](finite-heat-bath.md) example and the stipulated $G=2\,\mathrm{W\,K^{-1}}=2\,\mathrm{J\,s^{-1}\,K^{-1}}$, $\tau=45\,\mathrm s$, and solving the [ordinary differential equations](ordinary-differential-equation.md) gives

$$
T_1(t)=296\,\mathrm K+54\,\mathrm K\,e^{-t/(45\,\mathrm s)},\qquad
T_2(t)=296\,\mathrm K-6\,\mathrm K\,e^{-t/(45\,\mathrm s)},
$$



$$
Q(t)=5400\,\mathrm J\left(1-e^{-t/(45\,\mathrm s)}\right).
$$

At one [time constant](time-constant.md), $T_1\simeq315.865\,\mathrm K$, $T_2\simeq293.793\,\mathrm K$ and $Q\simeq3413.451\,\mathrm J$. Equal [temperatures](temperature-split.md) are approached as a [limit](limit-of-a-function.md) at infinite time. The finite bath causes the [temperature](temperature-split.md) difference to shrink faster than the fixed-bath model, because both bodies change [temperature](temperature-split.md).

<a id="image-finite-bath-and-fixed-bath-newton-s-law-of-cooling-histories"></a>
![](finite-heat-bath-newton-cooling.png)

**[Figure 3](#image-finite-bath-and-fixed-bath-newton-s-law-of-cooling-histories). Finite bath and fixed bath Newton's law of cooling histories**. Original analytical model predictions with $C_1=100\,\mathrm{J\,K^{-1}}$, $C_2=900\,\mathrm{J\,K^{-1}}$ and $G=2\,\mathrm{W\,K^{-1}}$; time is in seconds. Solid lines show the two finite bodies approaching $296\,\mathrm K$ with [time constant](time-constant.md) $45\,\mathrm s$. Dashed lines show body 1 cooling toward a bath held at $290\,\mathrm K$, with [time constant](time-constant.md) $50\,\mathrm s$. The two panels use different vertical scales so that the finite bath's $6\,\mathrm K$ warming remains visible.

For an ideal [heat bath](heat-bath.md) with the same $G$, set $T_2=T_b=290\,\mathrm K$ rather than evolving its [temperature](temperature-split.md). [Newton's law of cooling](newton-s-law-of-cooling.md) then yields

$$
T_1(t)=290\,\mathrm K+60\,\mathrm K\,e^{-t/(50\,\mathrm s)},\qquad
\tau_\infty=C_1/G=50\,\mathrm s.
$$

Changing $G$ changes these [time constants](time-constant.md), while the final [temperature](temperature-split.md) is fixed by the capacities and initial conditions. The dynamical model independently checks the [Second law of thermodynamics](second-law-of-thermodynamics-split.md):

$$
\dot S_{\rm tot}=\frac{-\dot Q}{T_1}+\frac{\dot Q}{T_2}
=\frac{G(T_1-T_2)^2}{T_1T_2}\ge0.
$$

Its [integral](integral-split.md) over the relaxation reproduces the endpoint [entropy](entropy-split.md) change. The useful separation is between capacity, which governs how much the bath [temperature](temperature-split.md) shifts, and [thermal conductance](thermal-conductance.md), which governs the exchange rate. Neither alone establishes a reliable [heat bath](heat-bath.md).

## ↑ Ancestors (8)

1. [Finite heat bath](finite-heat-bath.md)
2. [Heat bath](heat-bath.md)
3. [Thermal equilibrium](thermal-equilibrium-split.md)
4. [Thermodynamics](thermodynamics-split.md)
5. [Statistical physics](statistical-physics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)
