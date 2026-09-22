# Ideal-vapor Clausius-Clapeyron approximation

↑ **Parent:** [Clausius-Clapeyron relation](clausius-clapeyron-relation.md)

For [liquid](liquid.md)–[gas](gas.md) [phase coexistence](phase-coexistence.md), make two distinct approximations: the [gas](gas.md) obeys the [ideal gas law](ideal-gas-law.md), $v_{m,g}=RT/p$, and its [molar volume](molar-volume.md) greatly exceeds the [liquid](liquid.md) [molar volume](molar-volume.md), $v_{m,g}\gg v_{m,l}$. Here $R$ is the [molar gas constant](molar-gas-constant.md) and $p$ is the [saturation pressure](vapor-pressure.md) of the pure substance. Substitution into the [Clapeyron equation](clausius-clapeyron-relation.md) gives

$$
\frac{dp}{dT}\simeq\frac{L_m(T)p}{RT^2},\qquad \frac{d\ln(p/p_*)}{dT}\simeq\frac{L_m(T)}{RT^2},
$$

where $p_*>0$ is any fixed reference [pressure](pressure.md), making the [logarithm](logarithm.md) dimensionless. Constant [latent heat](latent-heat.md) is a further approximation, needed for the elementary [Integrated Clausius-Clapeyron relation](integrated-clausius-clapeyron-relation.md) below.[§5.1.2, “An Approximate Solution to the Clausius-Clapeyron Equation”: the three assumptions and the exponential solution](statistical-physics-by-david-tong.md)

The neglected [liquid](liquid.md) [molar volume](molar-volume.md) has a transparent error estimate. If the [gas](gas.md) is ideal but $\epsilon=v_{m,l}/v_{m,g}$ is retained, then

$$
\left(\frac{dp}{dT}\right)_{\rm full}=\frac{L_m p}{RT^2(1-\epsilon)},\qquad \frac{(dp/dT)_{\rm approx}}{(dp/dT)_{\rm full}}=1-\epsilon.
$$

Thus ignoring the [liquid](liquid.md) [molar volume](molar-volume.md) underestimates this slope by a relative amount $\epsilon$. This estimate does not bound errors from treating a [real gas](real-gas.md) as ideal or from freezing $L_m(T)$. Near a [thermodynamic critical point](thermodynamic-critical-point.md), the [gas](gas.md) and [liquid](liquid.md) [molar volumes](molar-volume.md) approach each other and these dilute-vapor assumptions fail.

**Table of contents**

- [Integrated Clausius-Clapeyron relation](integrated-clausius-clapeyron-relation.md)
  - [Stipulated vapor-pressure calculation](stipulated-vapor-pressure-calculation.md)
  - [Latent heat from a vapor-pressure slope](latent-heat-from-a-vapor-pressure-slope.md)

## ↑ Ancestors (11)

1. [Clausius-Clapeyron relation](clausius-clapeyron-relation.md)
2. [Latent heat](latent-heat.md)
3. [Phase coexistence curve](phase-coexistence-curve.md)
4. [Gibbs free energy](gibbs-free-energy.md)
5. [Thermodynamic free energy](thermodynamic-free-energy.md)
6. [Thermodynamic potential](thermodynamic-potential.md)
7. [Thermodynamics](thermodynamics-split.md)
8. [Statistical physics](statistical-physics-split.md)
9. [Branches of physics](branches-of-physics.md)
10. [Physics](physics-split.md)
11. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Integrated Clausius-Clapeyron relation](integrated-clausius-clapeyron-relation.md)
- [Latent heat from a vapor-pressure slope](latent-heat-from-a-vapor-pressure-slope.md)
- [Stipulated vapor-pressure calculation](stipulated-vapor-pressure-calculation.md)
