# Integrated Clausius-Clapeyron relation

↑ **Parent:** [Ideal-vapor Clausius-Clapeyron approximation](ideal-vapor-clausius-clapeyron-approximation.md)

If the molar [latent heat](latent-heat.md) $L_m$ is approximately constant on the chosen [temperature](temperature-split.md) interval, the [ideal-vapor Clausius-Clapeyron approximation](ideal-vapor-clausius-clapeyron-approximation.md) integrates to

$$
\ln\frac{p_2}{p_1}\simeq-\frac{L_m}{R}\left(\frac{1}{T_2}-\frac{1}{T_1}\right),\qquad p(T)\simeq p_1\exp\left[\frac{L_m}{R}\left(\frac{1}{T_1}-\frac{1}{T}\right)\right].
$$

For $L_m>0$, higher absolute [temperature](temperature-split.md) gives higher [saturation pressure](vapor-pressure.md). A plot of $\ln(p/p_1)$ against [inverse temperature](inverse-temperature.md) $1/T$ is a straight line of slope $-L_m/R$. One reference pair $(T_1,p_1)$ fixes its intercept. On a per-unit-[mass](mass.md) basis replace $L_m/R$ by $L/R_s$, with $R_s=R/M$ and $M$ the [molar mass](molar-mass.md); using $L$ in $\mathrm{J\,kg^{-1}}$ with the molar $R$ would give incompatible units.

If only the constant-[latent heat](latent-heat.md) approximation is relaxed, the same ideal-vapor model instead gives

$$
\ln\frac{p_2}{p_1}\simeq\frac{1}{R}\int_{T_1}^{T_2}\frac{L_m(T)}{T^2}\,dT.
$$

Consequently an apparent straight-line fit across a broad [temperature](temperature-split.md) range need not represent a single material constant. The simple exponential also approaches a finite value as $T\to\infty$; this is a property of the stipulated formula, not a prediction that [liquid](liquid.md)–[gas](gas.md) [phase coexistence](phase-coexistence.md) extends beyond a [thermodynamic critical point](thermodynamic-critical-point.md).

**Table of contents**

- [Stipulated vapor-pressure calculation](stipulated-vapor-pressure-calculation.md)
- [Latent heat from a vapor-pressure slope](latent-heat-from-a-vapor-pressure-slope.md)

## ↑ Ancestors (12)

1. [Ideal-vapor Clausius-Clapeyron approximation](ideal-vapor-clausius-clapeyron-approximation.md)
2. [Clausius-Clapeyron relation](clausius-clapeyron-relation.md)
3. [Latent heat](latent-heat.md)
4. [Phase coexistence curve](phase-coexistence-curve.md)
5. [Gibbs free energy](gibbs-free-energy.md)
6. [Thermodynamic free energy](thermodynamic-free-energy.md)
7. [Thermodynamic potential](thermodynamic-potential-split.md)
8. [Thermodynamics](thermodynamics-split.md)
9. [Statistical physics](statistical-physics-split.md)
10. [Branches of physics](branches-of-physics.md)
11. [Physics](physics-split.md)
12. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Cloud-chamber expansion model](cloud-chamber-expansion-model.md)
- [Ideal-vapor Clausius-Clapeyron approximation](ideal-vapor-clausius-clapeyron-approximation.md)
- [Vapor pressure](vapor-pressure.md)
