# Calorimeter heat-loss correction

↑ **Parent:** [Calorimeter](calorimeter.md)

A calorimeter heat-loss correction estimates the signed [heat](heat.md) exchanged with the room during the measurement. Under [Newton's law of cooling](newton-s-law-of-cooling.md), a constant room [temperature](temperature.md) $T_a$ and a single representative assembly [temperature](temperature.md) $T$ give the model

$$
C_{\rm eff}\frac{dT}{dt}=P(t)-G(T-T_a),\qquad
Q_{\rm loss,out}=G\int_{t_0}^{t_1}(T(t)-T_a)\,dt.
$$

Here $P(t)$ is deposited input [power](power.md), and $G$ is the apparatus loss coefficient in $\mathrm{W\,K^{-1}}$. After input ceases, the [temperature](temperature.md) excess shows [exponential decay](exponential-decay.md) with [time constant](time-constant.md) $\tau=C_{\rm eff}/G$:

$$
T(t)-T_a=(T(t_1)-T_a)e^{-(t-t_1)/\tau}.
$$

A cooling trace determines the ratio $G/C_{\rm eff}$, not the two factors separately. Combining the cooling trace with a known electrical [energy](energy.md) input supplies the missing information. For constant input $P_0$, starting at $T_a$, the heating solution is $T(t)-T_a=(P_0/G)(1-e^{-t/\tau})$; these solutions generate the calibration figure.

For [mixing calorimetry](mixing-calorimetry.md), infer cooling behavior only after the sample, [water](water.md) and vessel approach a common [temperature](temperature.md). Applying a single-body cooling model while the sample remains much hotter than the [water](water.md) can misestimate the earlier loss. The Toronto handout's area correction assumes the same loss mechanism represents both the mixing interval and subsequent cooling.[p. 3, Figure 1 and the area-ratio cooling correction](heat-capacity-university-of-toronto-laboratory-handout.md) A backward extrapolation to the transfer time is therefore a model-dependent estimate, not the ultimate equilibrium with the room. Extend the model or report a limitation if sensor delay, substantial [temperature gradients](temperature-gradient.md), changing room [temperature](temperature.md), or escaping material invalidate that assumption. In particular, the relevant $C_{\rm eff}$ after adding a sample includes its [heat capacity](heat-capacity.md); an empty-receiver cooling rate need not apply to the loaded receiver.

## ↑ Ancestors (7)

1. [Calorimeter](calorimeter.md)
2. [Calorimetry](calorimetry.md)
3. [Thermodynamics](thermodynamics-split.md)
4. [Statistical physics](statistical-physics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Calorimeter calibration](calorimeter-calibration.md)
- [Electrical calorimetry of a resistor](electrical-calorimetry-of-a-resistor.md)
