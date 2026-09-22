<h1 id="angstrom-periodic-heating-method">Ångström periodic heating method</h1>

↑ **Parent:** [Thermal diffusivity](thermal-diffusivity.md)

The [Ångström periodic heating method](angstrom-periodic-heating-method.md) measures [thermal diffusivity](thermal-diffusivity.md) by periodically heating one end of a rod and comparing the resulting [temperature](temperature-split.md) oscillations at two separated [thermometers](thermometer.md). The farther signal has a smaller [amplitude](wave-amplitude.md) and a later [wave phase](phase-waves.md). Their combination measures how quickly the material redistributes [heat](heat-split.md), without requiring the absolute heater [power](power.md). The method bears the name of [Anders Jonas Ångström](anders-jonas-angstrom.md), the [physicist](physicist-split.md) who became a professor at Uppsala in 1858.[Uppsala University, Anders Ångström: appointment to professor of physics in 1858](anders-angstrom-by-uppsala-university.md)

An actual teaching apparatus is PASCO's TD-8513: four metal bars share a heater/cooler using the [thermoelectric effect](thermoelectric-effect-split.md), and each has two embedded [thermistors](thermistor.md) about $3\,\mathrm{cm}$ apart. Foam covers reduce environmental [heat transfer](heat-transfer.md). Its manual instructs students to measure sensor spacing and connect the [thermistors](thermistor.md) through a temperature interface to a computer. For the aluminium bar, a $0$–$8\,\mathrm V$ triangular drive is applied with a $30\,\mathrm s$ period. Recording begins after the [amplitudes](wave-amplitude.md) stabilize; two cycles provide [amplitudes](wave-amplitude.md) and the delay between corresponding peaks. Repeated runs at $40$ and $50\,\mathrm s$ test consistency. The manual converts the inferred [thermal diffusivity](thermal-diffusivity.md) to [thermal conductivity](thermal-conductivity.md) using [mass density](density.md) and [specific heat capacity](specific-heat-capacity.md).[PASCO scientific, Heat Conduction Apparatus TD-8513 Instruction Manual, p. 3 Introduction; pp. 9–11 Experiment 2: apparatus, amplitude/phase inference and aluminium procedure](heat-conduction-apparatus-td-8513-instruction-manual-by-pasco-scientific.md)

For a general rod experiment, attach small [thermocouples](thermocouple.md), [thermistors](thermistor.md) or other [thermometers](thermometer.md) at measured positions $x_1<x_2$, record both against the same clock, and establish a [steady periodic thermal state](steady-periodic-thermal-state.md). A [sinusoid](sinusoid.md) is especially convenient. For a switched or triangular drive, isolate the same [Fourier series](fourier-series-split.md) component at both sensors: unrelated peaks in distorted waveforms need not measure that component's [phase difference](phase-difference.md). Subtract each sensor's mean [temperature](temperature-split.md); a steady spatial background does not belong in the oscillating [amplitude](wave-amplitude.md) ratio. Small excursions help keep [thermal conductivity](thermal-conductivity.md), [mass density](density.md) and [specific heat capacity](specific-heat-capacity.md) constant.

<a id="image-angstrom-periodic-heating-method-geometry-spaced-thermometers-and-possible-side-losses"></a>
![](angstrom-periodic-heating-rod-geometry.png)

**[Figure 5](#image-angstrom-periodic-heating-method-geometry-spaced-thermometers-and-possible-side-losses). Ångström periodic heating method: geometry, spaced thermometers and possible side losses**. Original idealized rod geometry, rather than a scale reconstruction of the PASCO apparatus. Either a heater/cooler or a heater modulated about a mean input establishes the oscillating [temperature](temperature-split.md). Sensor spacing fixes the [length](length.md) used in the inference. The two channels must measure the same [angular frequency](angular-frequency.md) with calibrated relative [amplitude](wave-amplitude.md) and [wave phase](phase-waves.md).

The appeal is that the rod supplies two complementary clocks: decreasing [amplitude](wave-amplitude.md) measures spatial damping, while increasing [wave phase](phase-waves.md) lag measures delay. Unlike [laser flash analysis](laser-flash-analysis.md), which follows a transient after one pulse, this method repeatedly samples a [steady periodic thermal state](steady-periodic-thermal-state.md). The timing determines [thermal diffusivity](thermal-diffusivity.md) $\alpha$ in $\mathrm{m^2\,s^{-1}}$. To infer [thermal conductivity](thermal-conductivity.md) $k$ in $\mathrm{W\,m^{-1}\,K^{-1}}$, also measure or otherwise justify the [mass density](density.md) $\rho$ and [specific heat capacity at constant pressure](specific-heat-capacity-at-constant-pressure.md) $c_p$:

$$
k=\rho c_p\alpha.
$$

Here the stationary-solid approximation neglects thermal expansion and mechanical [work](work.md), as in [thermal diffusivity](thermal-diffusivity.md). A timing measurement alone cannot distinguish two materials with the same $\alpha$ and different [volumetric heat capacities](volumetric-heat-capacity.md).

**Table of contents**

- [Steady periodic thermal state](steady-periodic-thermal-state.md)
- [Thermal diffusion wave](thermal-diffusion-wave.md)
  - [Thermal penetration depth](thermal-penetration-depth.md)
- [Ångström method with linear heat loss](angstrom-method-with-linear-heat-loss.md)
- [Ångström method worked example](angstrom-method-worked-example.md)
- [Finite-end correction for periodic rod heating](finite-end-correction-for-periodic-rod-heating.md)

## ↑ Ancestors (8)

1. [Thermal diffusivity](thermal-diffusivity.md)
2. [Thermal conduction](thermal-conduction.md)
3. [Heat](heat-split.md)
4. [Thermodynamics](thermodynamics-split.md)
5. [Statistical physics](statistical-physics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Ångström periodic heating method](angstrom-periodic-heating-method.md)
