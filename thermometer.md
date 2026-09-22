# Thermometer

↑ **Parent:** [Temperature](temperature-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Thermometer)

A thermometer measures [temperature](temperature-split.md) through a physical response whose relation to [temperature](temperature-split.md) is known. Examples include the length change from [thermal expansion](thermal-expansion.md), a change in [electrical resistance](electrical-resistance.md), and the [pressure](pressure-split.md) of a [gas thermometer](gas-thermometer.md). If the response [function](function-split.md) $X=f(T)$ is an [injective function](injective-function.md) over the working range, its measured value determines $T=f^{-1}(X)$ through the [inverse function](inverse-function.md). [Thermometer calibration](thermometer-calibration.md) establishes that relation for the particular instrument and measurement conditions. Two matching readings are meaningful only after calibration to a common scale and with the probes sampling comparable equilibrium states. [Ling, Moebs and Sanny, University Physics Volume 2, section 1.2: physical responses used in thermometers](https://openstax.org/books/university-physics-volume-2/pages/1-2-thermometers-and-temperature-scales)

For a contact thermometer, the sensing part must reach [thermal equilibrium](thermal-equilibrium-split.md) with the region being measured. That region may differ from the rest of the object: an immersed probe near a heater can read a local [temperature](temperature-split.md) while the surrounding [water](water.md) remains cooler. A stable reading can also be a [steady state](steady-state.md) set by competing [heat transfer](heat-transfer.md) paths to the sample and the room. Good contact, adequate immersion, mixing where appropriate, and checks for spatial differences help establish which [temperature](temperature-split.md) the reading represents. These are measurement controls inferred from the [thermal equilibrium](thermal-equilibrium-split.md) requirement, not a guarantee that every flat trace is equilibrium.

A thermometer also changes the sample it touches. Consider an original toy calculation with an initially uniform sample at $T_o=350\,\mathrm K$, a probe at $T_p=300\,\mathrm K$, and constant whole-body [heat capacities](heat-capacity.md) $C_o=100\,\mathrm{J\,K^{-1}}$ and $C_p=1\,\mathrm{J\,K^{-1}}$. Suppose together they form an [isolated system](isolated-system.md), with no [work](work.md) or [phase transition](phase-transition.md) and negligible contact [energy](energy-split.md). The [first law of thermodynamics](first-law-of-thermodynamics-split.md) and [thermal equilibrium](thermal-equilibrium-split.md) give

$$
T_f=\frac{C_oT_o+C_pT_p}{C_o+C_p}=349.50495\ldots\,\mathrm K,\qquad
T_f-T_o=\frac{C_p}{C_o+C_p}(T_p-T_o).
$$

The final [thermometer](thermometer.md) reading underestimates the sample's original [temperature](temperature-split.md) by about $0.495\,\mathrm K$, although it correctly measures their new common [temperature](temperature-split.md). The disturbance becomes small when the participating probe [heat capacity](heat-capacity.md) is small compared with the sample's. A large controlled [heat bath](heat-bath.md) is a different limit: it supplies or removes [heat](heat-split.md) while approximately maintaining its own [temperature](temperature-split.md).

Waiting time is a separate issue from disturbance. Under a toy [Newton's law of cooling](newton-s-law-of-cooling.md) model for a uniform probe in a maintained [heat bath](heat-bath.md), a constant contact conductance $G$ gives

$$
C_p\frac{dT_p}{dt}=G(T_b-T_p),\qquad
T_p(t)=T_b+[T_p(0)-T_b]e^{-t/\tau},\qquad \tau=\frac{C_p}{G}.
$$

The [time constant](time-constant.md) $\tau$ controls this [exponential decay](exponential-decay.md). For stipulated values $T_b=350\,\mathrm K$, $T_p(0)=300\,\mathrm K$ and $\tau=5\,\mathrm s$, the probe reads about $331.61\,\mathrm K$ after one [time constant](time-constant.md) and $347.51\,\mathrm K$ after three. These are calculated values, not an instrument specification or measured data. Real probes may have multiple relaxation times and additional [heat transfer](heat-transfer.md) paths; choose an equilibration criterion from the required accuracy, rather than assuming that a fixed waiting time works universally.

**Table of contents**

- [Resistance thermometer](resistance-thermometer.md)
  - [Platinum resistance thermometer](platinum-resistance-thermometer.md)
    - [Standard platinum resistance thermometer](standard-platinum-resistance-thermometer.md)
    - [Industrial platinum resistance thermometer](industrial-platinum-resistance-thermometer.md)
      - [Pt100](pt100.md)
        - [Pt100 local linear model](pt100-local-linear-model.md)
    - [Platinum resistance thermometer comparison calibration](platinum-resistance-thermometer-comparison-calibration.md)
    - [Platinum resistance thermometer lead resistance error](platinum-resistance-thermometer-lead-resistance-error.md)
  - [Resistance thermometer self-heating](resistance-thermometer-self-heating.md)
  - [Resistance thermometer immersion test](resistance-thermometer-immersion-test.md)
  - [Thermistor](thermistor.md)
- [Gas thermometer](gas-thermometer.md)
  - [Gas thermometer dead-space correction](gas-thermometer-dead-space-correction.md)
- [Thermometer calibration](thermometer-calibration.md)

## ↑ Ancestors (6)

1. [Temperature](temperature-split.md)
2. [Thermodynamics](thermodynamics-split.md)
3. [Statistical physics](statistical-physics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (64)

- [Adiabatic process](adiabatic-process.md)
- [Andrews's carbon dioxide experiment](andrews-s-carbon-dioxide-experiment.md)
- [Ångström method worked example](angstrom-method-worked-example.md)
- [Ångström periodic heating method](angstrom-periodic-heating-method.md)
- [Boltzmann distribution](boltzmann-distribution.md)
- [Calorimeter](calorimeter.md)
- [Calorimeter addenda](calorimeter-addenda.md)
- [Cold-junction compensation](cold-junction-compensation.md)
- [Distillation](distillation.md)
- [Electrical calorimetry of a resistor](electrical-calorimetry-of-a-resistor.md)
- [Electrical substitution radiometer](electrical-substitution-radiometer.md)
- [Empirical temperature](empirical-temperature.md)
- [Flat-plate boundary-layer traverse experiment](flat-plate-boundary-layer-traverse-experiment.md)
- [Fourth-power thermal boundary model](fourth-power-thermal-boundary-model.md)
- [Free expansion](free-expansion.md)
- [Gas thermometer](gas-thermometer.md)
- [George T. Furukawa](george-t-furukawa.md)
- [Giauque-MacDougall magnetic cooling experiment](giauque-macdougall-magnetic-cooling-experiment.md)
- [Heat-pump calorimetry](heat-pump-calorimetry.md)
- [Hess's law calorimetry experiment](hess-s-law-calorimetry-experiment.md)
- [Ice-melting calorimetry](ice-melting-calorimetry.md)
- [Infrared](infrared.md)
- [Isothermal terminal block](isothermal-terminal-block.md)
- [Joule's free-expansion experiment](joule-s-free-expansion-experiment.md)
- [Joule's paddle-wheel experiment](joule-s-paddle-wheel-experiment.md)
- [Kamerlingh Onnes's 1908 helium liquefaction experiment](kamerlingh-onnes-s-1908-helium-liquefaction-experiment.md)
- [Kapitza thermal boundary experiment](kapitza-thermal-boundary-experiment.md)
- [Kundt tube experiment](kundt-tube-experiment.md)
- [Latent heat of fusion](latent-heat-of-fusion.md)
- [Lattice enthalpy from solution calorimetry](lattice-enthalpy-from-solution-calorimetry.md)
- [Low-temperature heat capacity measurement](low-temperature-heat-capacity-measurement.md)
- [Mechanical input and thermal storage in a calorimeter](mechanical-input-and-thermal-storage-in-a-calorimeter.md)
- [Meissner effect discovery](meissner-effect-discovery.md)
- [Michelson measurement of length in cadmium wavelengths](michelson-measurement-of-length-in-cadmium-wavelengths.md)
- [Nambu superconductivity and chiral symmetry analogy](nambu-superconductivity-and-chiral-symmetry-analogy.md)
- [Observation of Fermi pressure in trapped lithium](observation-of-fermi-pressure-in-trapped-lithium.md)
- [Optical-electrical heating non-equivalence](optical-electrical-heating-non-equivalence.md)
- [Paddle-wheel calorimetry energy balance](paddle-wheel-calorimetry-energy-balance.md)
- [Paired simple and fractional distillation experiment](paired-simple-and-fractional-distillation-experiment.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-1/section-d/d13/b/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2019/paper-2/section-c/c13/solution.md)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2015/paper-1/2/c/solution.md)
- [Peltier current-reversal experiment](peltier-current-reversal-experiment.md)
- [Reference-bath thermometer comparison](reference-bath-thermometer-comparison.md)
- [Regulated calibration bath](regulated-calibration-bath.md)
- [Resistance thermometer](resistance-thermometer.md)
- [Resistance thermometer immersion test](resistance-thermometer-immersion-test.md)
- [Resistance-versus-temperature experiment for superconductivity](resistance-versus-temperature-experiment-for-superconductivity.md)
- [Solvation thermodynamic balance](solvation-thermodynamic-balance.md)
- [Standard platinum resistance thermometer](standard-platinum-resistance-thermometer.md)
- [Temperature](temperature-split.md)
- [Thermal boundary resistance](thermal-boundary-resistance.md)
- [Thermal equilibrium](thermal-equilibrium-split.md)
- [Thermal transpiration experiment with a glass microtube](thermal-transpiration-experiment-with-a-glass-microtube.md)
- [Thermocouple reference function](thermocouple-reference-function.md)
- [Thermocouple voltage calibration](thermocouple-voltage-calibration.md)
- [Thermometer](thermometer.md)
- [Thermometer calibration](thermometer-calibration.md)
- [Triple-point cell](triple-point-cell.md)
- [Two-point thermometer calibration example](two-point-thermometer-calibration-example.md)
- [Ultraviolet](ultraviolet.md)
- [Vapor-density molar mass measurement](vapor-density-molar-mass-measurement.md)
- [Zeroth law of thermodynamics](zeroth-law-of-thermodynamics.md)
- [Zeroth-law thermometer comparison](zeroth-law-thermometer-comparison.md)
