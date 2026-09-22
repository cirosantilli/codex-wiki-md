# Finite-rate isothermal piston model

↑ **Parent:** [Isothermal process](isothermal-process.md)

Why must a conducting piston move slowly? A simple model couples the [first law of thermodynamics](first-law-of-thermodynamics.md) to [Newton's law of cooling](newton-s-law-of-cooling.md). Assume a fixed amount of [ideal gas](ideal-gas.md) with uniform [temperature](temperature.md) $T(t)$ and constant whole-sample [heat capacity at constant volume](heat-capacity-at-constant-volume.md) $C_V$, a [heat bath](heat-bath.md) maintained at $T_b$, negligible [friction](friction.md), and mechanically slow motion. Let $G>0$ be the effective thermal conductance, the reciprocal of the [thermal resistance](thermal-resistance.md), in $\mathrm{W\,K^{-1}}$. Then

$$
\dot Q=G(T_b-T),\qquad p=\frac{nRT}{V},\qquad
C_V\dot T=G(T_b-T)-p\dot V.
$$

Positive [heat transfer](heat-transfer.md) must offset expansion [work](work.md) to keep $T$ near $T_b$. A finite $G$ and nonzero piston speed therefore require a [temperature](temperature.md) difference. This uniform-[temperature](temperature.md) model neglects spatial [temperature gradients](temperature-gradient.md), sensor response, cylinder [heat capacity](heat-capacity.md) and any change of $G$ with piston position; it is an illustrative calculation, not a fit to the [isothermal gas syringe experiment](isothermal-gas-syringe-experiment.md).

<a id="image-conducting-piston-in-a-thermal-bath-and-modeled-temperature-lag-during-expansion"></a>
![](isothermal-piston-thermal-bath-temperature-lag.png)

**[Figure 30](#image-conducting-piston-in-a-thermal-bath-and-modeled-temperature-lag-during-expansion). Conducting piston in a thermal bath and modeled temperature lag during expansion**.

For a prescribed exponential [volume](volume-thermodynamics.md) change $V=V_i e^{\lambda t}$, define $\tau=C_V/G$, $s=t/\tau$ and $\epsilon=nR\lambda/G$. The dimensionless [temperature](temperature.md) $\theta=T/T_b$ obeys a [linear ordinary differential equation](linear-ordinary-differential-equation.md) with initial value $\theta(0)=1$:

$$
\frac{d\theta}{ds}=1-(1+\epsilon)\theta,\qquad
\theta(s)=\frac{1}{1+\epsilon}
+\frac{\epsilon}{1+\epsilon}e^{-(1+\epsilon)s}.
$$

The plotted expansion uses stipulated $C_V=(5/2)nR$ and stops at $V_f=2V_i$, at $s_f=\ln2/[(5/2)\epsilon]$. During expansion, the larger $\epsilon$ produces the larger [temperature](temperature.md) deficit; once the piston is held fixed, the deficit undergoes [exponential decay](exponential-decay.md) as $e^{-(s-s_f)}$. Reducing $|\epsilon|$ makes the path more nearly an [isothermal process](isothermal-process.md), while increasing its duration. Reversing the piston with $\lambda<0$ produces a [temperature](temperature.md) excess and outward [heat transfer](heat-transfer.md); the small-$|\epsilon|$ regime is the intended near-isothermal approximation. Mechanical slowness alone does not ensure sufficient [heat transfer](heat-transfer.md).

## ↑ Ancestors (9)

1. [Isothermal process](isothermal-process.md)
2. [Carnot cycle](carnot-cycle.md)
3. [Carnot's theorem](carnot-s-theorem.md)
4. [Second law of thermodynamics](second-law-of-thermodynamics.md)
5. [Thermodynamics](thermodynamics-split.md)
6. [Statistical physics](statistical-physics-split.md)
7. [Branches of physics](branches-of-physics.md)
8. [Physics](physics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Isothermal compression](isothermal-compression.md)
- [Isothermal process](isothermal-process.md)
