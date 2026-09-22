# Thermometer

↑ **Parent:** [Temperature](temperature.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Thermometer)

A thermometer measures [temperature](temperature.md) through a physical response whose relation to [temperature](temperature.md) is known. Examples include the length change from [thermal expansion](thermal-expansion.md), a change in [electrical resistance](electrical-resistance.md), and the [pressure](pressure.md) of a [gas thermometer](gas-thermometer.md). If the response [function](function-split.md) $X=f(T)$ is an [injective function](injective-function.md) over the working range, its measured value determines $T=f^{-1}(X)$ through the [inverse function](inverse-function.md). [Thermometer calibration](thermometer-calibration.md) establishes that relation for the particular instrument and measurement conditions. Two matching readings are meaningful only after calibration to a common scale and with the probes sampling comparable equilibrium states. [Ling, Moebs and Sanny, University Physics Volume 2, section 1.2: physical responses used in thermometers](https://openstax.org/books/university-physics-volume-2/pages/1-2-thermometers-and-temperature-scales)

For a contact thermometer, the sensing part must reach [thermal equilibrium](thermal-equilibrium.md) with the region being measured. That region may differ from the rest of the object: an immersed probe near a heater can read a local [temperature](temperature.md) while the surrounding [water](water.md) remains cooler. A stable reading can also be a [steady state](steady-state.md) set by competing [heat transfer](heat-transfer.md) paths to the sample and the room. Good contact, adequate immersion, mixing where appropriate, and checks for spatial differences help establish which [temperature](temperature.md) the reading represents. These are measurement controls inferred from the [thermal equilibrium](thermal-equilibrium.md) requirement, not a guarantee that every flat trace is equilibrium.

A thermometer also changes the sample it touches. Consider an original toy calculation with an initially uniform sample at $T_o=350\,\mathrm K$, a probe at $T_p=300\,\mathrm K$, and constant whole-body [heat capacities](heat-capacity.md) $C_o=100\,\mathrm{J\,K^{-1}}$ and $C_p=1\,\mathrm{J\,K^{-1}}$. Suppose together they form an [isolated system](isolated-system.md), with no [work](work.md) or [phase transition](phase-transition.md) and negligible contact [energy](energy.md). The [first law of thermodynamics](first-law-of-thermodynamics.md) and [thermal equilibrium](thermal-equilibrium.md) give

$$
T_f=\frac{C_oT_o+C_pT_p}{C_o+C_p}=349.50495\ldots\,\mathrm K,\qquad
T_f-T_o=\frac{C_p}{C_o+C_p}(T_p-T_o).
$$

The final [thermometer](thermometer.md) reading underestimates the sample's original [temperature](temperature.md) by about $0.495\,\mathrm K$, although it correctly measures their new common [temperature](temperature.md). The disturbance becomes small when the participating probe [heat capacity](heat-capacity.md) is small compared with the sample's. A large controlled [heat bath](heat-bath.md) is a different limit: it supplies or removes [heat](heat.md) while approximately maintaining its own [temperature](temperature.md).

Waiting time is a separate issue from disturbance. Under a toy [Newton's law of cooling](newton-s-law-of-cooling.md) model for a uniform probe in a maintained [heat bath](heat-bath.md), a constant contact conductance $G$ gives

$$
C_p\frac{dT_p}{dt}=G(T_b-T_p),\qquad
T_p(t)=T_b+[T_p(0)-T_b]e^{-t/\tau},\qquad \tau=\frac{C_p}{G}.
$$

The [time constant](time-constant.md) $\tau$ controls this [exponential decay](exponential-decay.md). For stipulated values $T_b=350\,\mathrm K$, $T_p(0)=300\,\mathrm K$ and $\tau=5\,\mathrm s$, the probe reads about $331.61\,\mathrm K$ after one [time constant](time-constant.md) and $347.51\,\mathrm K$ after three. These are calculated values, not an instrument specification or measured data. Real probes may have multiple relaxation times and additional [heat transfer](heat-transfer.md) paths; choose an equilibration criterion from the required accuracy, rather than assuming that a fixed waiting time works universally.

**Table of contents**

- [Resistance thermometer](resistance-thermometer.md)
  - [Platinum resistance thermometer](platinum-resistance-thermometer.md)
- [Gas thermometer](gas-thermometer.md)
  - [Gas thermometer dead-space correction](gas-thermometer-dead-space-correction.md)
- [Thermometer calibration](thermometer-calibration.md)

## ↑ Ancestors (6)

1. [Temperature](temperature.md)
2. [Thermodynamics](thermodynamics-split.md)
3. [Statistical physics](statistical-physics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (31)

- [Adiabatic process](adiabatic-process.md)
- [Andrews's carbon dioxide experiment](andrews-s-carbon-dioxide-experiment.md)
- [Boltzmann distribution](boltzmann-distribution.md)
- [Calorimeter](calorimeter.md)
- [Electrical calorimetry of a resistor](electrical-calorimetry-of-a-resistor.md)
- [Empirical temperature](empirical-temperature.md)
- [Flat-plate boundary-layer traverse experiment](flat-plate-boundary-layer-traverse-experiment.md)
- [Free expansion](free-expansion.md)
- [Gas thermometer](gas-thermometer.md)
- [Heat-pump calorimetry](heat-pump-calorimetry.md)
- [Ice-melting calorimetry](ice-melting-calorimetry.md)
- [Infrared](infrared.md)
- [Joule's free-expansion experiment](joule-s-free-expansion-experiment.md)
- [Joule's paddle-wheel experiment](joule-s-paddle-wheel-experiment.md)
- [Latent heat of fusion](latent-heat-of-fusion.md)
- [Lattice enthalpy from solution calorimetry](lattice-enthalpy-from-solution-calorimetry.md)
- [Meissner effect discovery](meissner-effect-discovery.md)
- [Paddle-wheel calorimetry energy balance](paddle-wheel-calorimetry-energy-balance.md)
- [Reference-bath thermometer comparison](reference-bath-thermometer-comparison.md)
- [Resistance thermometer](resistance-thermometer.md)
- [Resistance-versus-temperature experiment for superconductivity](resistance-versus-temperature-experiment-for-superconductivity.md)
- [Solvation thermodynamic balance](solvation-thermodynamic-balance.md)
- [Temperature](temperature.md)
- [Thermal equilibrium](thermal-equilibrium.md)
- [Thermal transpiration experiment with a glass microtube](thermal-transpiration-experiment-with-a-glass-microtube.md)
- [Thermometer](thermometer.md)
- [Thermometer calibration](thermometer-calibration.md)
- [Two-point thermometer calibration example](two-point-thermometer-calibration-example.md)
- [Ultraviolet](ultraviolet.md)
- [Zeroth law of thermodynamics](zeroth-law-of-thermodynamics.md)
- [Zeroth-law thermometer comparison](zeroth-law-thermometer-comparison.md)
