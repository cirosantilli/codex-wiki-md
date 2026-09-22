# Mixture measurements and the Gibbs-Duhem constraint

↑ **Parent:** [Gibbs-Duhem equation](gibbs-duhem-equation.md)

A concrete motivating experiment is the [acetone](acetone.md)–[chloroform](chloroform.md) [mixture](mixture-split.md) in Truman State University's Liquid-Vapor Equilibrium of a Binary System, Procedure and Figure 1. A two-neck flask feeds a [distillation](distillation.md) head with a water-cooled [laboratory condenser](laboratory-condenser.md), condensate sampling arm and [temperature](temperature-split.md) probe. Starting with one pure [liquid](liquid.md), the procedure adds the other component successively and waits for stable [temperature](temperature-split.md) with returning condensate. Small paired samples from the flask and condensate are read on an [Abbé refractometer](abbe-refractometer.md); a tabulated [refractive index](refractive-index.md)–composition relation gives the two compositions. Controls include three-point [thermometer calibration](thermometer-calibration.md), corrected atmospheric [pressure](pressure-split.md) readings, and agreement of the initial pure-[liquid](liquid.md) and condensate [refractive indices](refractive-index.md) with the reference value. Small withdrawals and little retained condensate reduce disturbance of composition. Sample [evaporation](evaporation.md) can bias the readout. The inferred paired [mole fractions](mole-fraction.md), [temperature](temperature-split.md) and [pressure](pressure-split.md) describe [vapor-liquid equilibrium](vapor-liquid-equilibrium.md), subject to the conversion from [mass fraction](mass-fraction.md) to [mole fraction](mole-fraction.md) and to representative sampling. This teaching protocol reports no measured results of a particular student run.[Liquid-Vapor Equilibrium of a Binary System, adapted by J. M. McCormick; Procedure, Figure 1, Tables 1–2, pure-solvent checks and repeated additions](liquid-vapor-equilibrium-of-a-binary-system-by-james-m-mccormick.md)

How does such a measurement expose [activity coefficients](activity-coefficient.md)? Let $x_i$ and $y_i$ be the [mole fractions](mole-fraction.md) in the [liquid](liquid.md) and [gas](gas.md) [thermodynamic phases](thermodynamic-phase.md), respectively, and let $p_i^*(T)$ be the pure-component [vapor pressure](vapor-pressure.md). Assume the [gas](gas.md) [thermodynamic phase](thermodynamic-phase.md) is an [ideal gas](ideal-gas-split.md) [mixture](mixture-split.md) and neglect the change of the pure-[liquid](liquid.md) reference [chemical potential](chemical-potential-split.md) between its saturation [pressure](pressure-split.md) and the experimental [pressure](pressure-split.md). Equality of each component's [chemical potential](chemical-potential-split.md) between the two [thermodynamic phases](thermodynamic-phase.md) then gives

$$
RT\ln(x_i\gamma_i)=RT\ln\frac{y_i p}{p_i^*(T)},
\qquad
\gamma_i\simeq\frac{y_i p}{x_i p_i^*(T)}.
$$

This turns the paired composition readings into estimates of the [activity coefficients](activity-coefficient.md). The approximation needs refinement when the [gas](gas.md) departs appreciably from [ideal gas](ideal-gas-split.md) behavior or the neglected [liquid](liquid.md) [pressure](pressure-split.md) effect matters.

The apparatus measures a boiling-composition series in which [temperature](temperature-split.md) changes as the [mixture](mixture-split.md) changes. Its readings therefore cannot be inserted directly into the fixed-[temperature](temperature-split.md), fixed-[pressure](pressure-split.md) [activity coefficient](activity-coefficient.md) constraint. They motivate the more general task: test whether the measured mixture properties can arise from a common [Gibbs free energy](gibbs-free-energy.md) while accounting for changing state variables. A failure can reveal incompatible property fits or experimental bias; a pass supplies a consistency check, not proof that every reading is correct.

## ↑ Ancestors (6)

1. [Gibbs-Duhem equation](gibbs-duhem-equation.md)
2. [Thermodynamics](thermodynamics-split.md)
3. [Statistical physics](statistical-physics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Ideal-solution vapor-liquid equilibrium test](ideal-solution-vapor-liquid-equilibrium-test.md)
