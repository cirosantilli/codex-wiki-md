# Ideal-solution vapor-liquid equilibrium test

↑ **Parent:** [Ideal solution](ideal-solution.md)

The [Mixture measurements and the Gibbs-Duhem constraint](mixture-measurements-and-the-gibbs-duhem-constraint.md) article describes the inspected [acetone](acetone.md)–[chloroform](chloroform.md) preparation, apparatus, paired readouts, controls and sampling limits.[Procedure, Figure 1, Tables 1–2: apparatus, calibration, pure-component control, successive additions and paired sampling](liquid-vapor-equilibrium-of-a-binary-system-by-james-m-mccormick.md)

That existing apparatus account supplies the experimental controls and limitations. Its [refractive index](refractive-index.md) calibration yields [mass fractions](mass-fraction.md), which must be converted to [mole fractions](mole-fraction.md). For a measured component-A [mass fraction](mass-fraction.md) $w_A$ and component [molar masses](molar-mass.md) $M_A,M_B$,

$$
x_A=\frac{w_A/M_A}{w_A/M_A+(1-w_A)/M_B}.
$$

Apply this conversion separately to the flask sample and to completely condensed [vapor](vapor.md) to obtain $x_A$ and $y_A$. Comparing $y_iP$ with $x_ip_i^*(T)$ tests [Raoult's law](raoult-s-law.md) at the measured [temperature](temperature-split.md); using the changing [temperature](temperature-split.md) at each composition is essential. The chosen A/B values above are unrelated to the protocol's substances.

The more general diagnostic, retaining an [ideal gas](ideal-gas-split.md) [vapor](vapor.md) and negligible pure-[liquid](liquid.md) [pressure](pressure-split.md) correction, is

$$
y_iP=x_i\gamma_i p_i^*(T),\qquad
\gamma_i\simeq\frac{y_iP}{x_ip_i^*(T)}.
$$

This follows by replacing $\ln x_i$ with $\ln(x_i\gamma_i)$ in the [chemical potential](chemical-potential-split.md) subtraction used for [Raoult's law](raoult-s-law.md). A reproducible discrepancy from $\gamma_i=1$ can expose failure of the [ideal solution](ideal-solution.md) approximation, but interpreting it requires checking [measurement uncertainty](measurement-uncertainty.md), representative paired sampling and the [ideal gas](ideal-gas-split.md) approximation. Apparent agreement within uncertainty supports an approximation over the tested conditions; it cannot establish exact ideality at every composition.

Positive or negative deviations of component [partial pressures](partial-pressure.md) require [activity coefficients](activity-coefficient.md) different from one under these assumptions. An [azeotrope](azeotrope.md) is also absent from the chosen unequal-[vapor pressure](vapor-pressure.md) model: the explicit inequality in [ideal binary vapor composition](ideal-binary-vapor-composition.md) gives $y_A>x_A$ throughout $0<x_A<1$. An interior equality would require $p_A^*=p_B^*$; in that degenerate case every composition has $y_A=x_A$, rather than an isolated enrichment reversal. Neither an [azeotrope](azeotrope.md) nor [liquid](liquid.md) [phase separation](phase-separation.md) should be inferred from the ideal curves.

## ↑ Ancestors (5)

1. [Ideal solution](ideal-solution.md)
2. [Solution (chemistry)](solution-chemistry.md)
3. [Mixture](mixture-split.md)
4. [Chemistry](chemistry-split.md)
5. [Codex Wiki](split.md)
