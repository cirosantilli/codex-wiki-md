# Adiabatic process

↑ **Parent:** [First law of thermodynamics](first-law-of-thermodynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Adiabatic_process)

An [adiabatic process](adiabatic-process.md) has no [heat transfer](heat-transfer.md) across the chosen boundary throughout the process: $\delta Q=0$, rather than merely zero net [heat](heat.md) after incoming and outgoing transfers cancel. It is a condition on [energy](energy.md) transfer, whereas an [isothermal process](isothermal-process.md) holds [temperature](temperature.md) constant. A sealed cylinder can approach an [adiabatic process](adiabatic-process.md) through insulation or through motion short compared with the time needed for appreciable [heat transfer](heat-transfer.md). Its [temperature](temperature.md) can nevertheless change because [work](work.md) crosses the boundary.[§§4.2–4.3: work, heat, and adiabatic legs of a cycle](statistical-physics-by-david-tong/4-classical-thermodynamics.md)

Take the trapped [gas](gas.md) as a [closed system](closed-system.md), with fixed [amount of substance](amount-of-substance.md) and composition and no net change in bulk [kinetic energy](kinetic-energy.md) or [potential energy](potential-energy.md) between the endpoints. Define $Q_{\rm in}>0$ as [heat](heat.md) entering and $W_{\rm out}>0$ as [work](work.md) delivered to the surroundings. The [first law of thermodynamics](first-law-of-thermodynamics.md) gives

$$
\Delta U=Q_{\rm in}-W_{\rm out},\qquad
Q_{\rm in}=0\ \Longrightarrow\ \Delta U=-W_{\rm out}.
$$

Here $U$ is [internal energy](internal-energy.md). An [adiabatic compression](adiabatic-compression.md) normally supplies [work](work.md), so $W_{\rm out}<0$; an [adiabatic expansion](adiabatic-expansion.md) against a resisting load delivers [work](work.md), so $W_{\rm out}>0$. An [adiabatic process](adiabatic-process.md) need not preserve [internal energy](internal-energy.md) and need not make the [closed system](closed-system.md) an [isolated system](isolated-system.md). [MIT Unified Engineering, §2.5.2: heat inward and work outward in the first-law balance](https://web.mit.edu/16.unified/www/FALL/thermodynamics/notes/node19.html)

For a [reversible thermodynamic process](reversible-thermodynamic-process.md), $dS=\delta Q_{\rm rev}/T$ at positive absolute [temperature](temperature.md) $T$. A reversible [adiabatic process](adiabatic-process.md) therefore has $dS=0$: it is an [isentropic process](isentropic-process.md). Irreversible [adiabatic processes](adiabatic-process.md) can instead generate [entropy](entropy.md); [free expansion](free-expansion.md) is the existing counterexample, with its calculation in [entropy change in free expansion](entropy-change-in-free-expansion.md). Conversely, constant [entropy](entropy.md) alone does not certify an [adiabatic process](adiabatic-process.md) or reversibility: outward [heat](heat.md) can export the [entropy](entropy.md) generated internally. For a [closed system](closed-system.md) the macroscopic [entropy](entropy.md) balance is

$$
\Delta S=\int\frac{\delta Q_{\rm in}}{T_b}+S_{\rm gen},\qquad S_{\rm gen}\geq0,
$$

where $T_b$ is the absolute boundary [temperature](temperature.md) where each [heat](heat.md) transfer occurs and $S_{\rm gen}$ is internal [entropy production](entropy-production.md). With no [heat transfer](heat-transfer.md), this reduces to $\Delta S=S_{\rm gen}$; reversibility makes $S_{\rm gen}=0$. [Ling, Moebs and Sanny, University Physics Volume 2, §4.6: reversible heat and irreversible entropy increase](https://openstax.org/books/university-physics-volume-2/pages/4-6-entropy)

A motivating experiment measures the [gas](gas.md) [temperature](temperature.md) directly during compression and expansion, instead of inferring it from how warm a cylinder feels. PASCO's authored TD-8565 manual describes a sealed piston cylinder, a fine nickel-wire [thermometer](thermometer.md), an absolute [pressure](pressure.md) sensor and a position readout for [volume](volume-thermodynamics.md). A computer records all three channels together. The wire's [electrical resistance](electrical-resistance.md) changes with [temperature](temperature.md); its small size permits a rapid response. [PASCO scientific, Adiabatic Gas Law Apparatus, guide 012-05110D, pp. 1–2: apparatus and readouts](https://cdn.pasco.com/product_document/Adiabatic-Gas-Law-Apparatus-TD-8565-Manual.pdf)

Use ordinary trapped air and the apparatus's designed travel stops; mount the base securely, close the valve during a stroke, and record the actual [volume](volume-thermodynamics.md) limits. John Hart's university demonstration uses a large transparent cylinder with a low-[heat capacity](heat-capacity.md) [thermocouple](thermocouple.md), a [pressure](pressure.md) sensor, a travel gauge and a safety stop. It explicitly keeps the release valve closed during the demonstration. The basic observable is a rise in [temperature](temperature.md) on compression and a fall on loaded expansion, alongside the corresponding [pressure](pressure.md) and [volume](volume-thermodynamics.md) changes. Hart discusses wall [thermal conduction](thermal-conduction.md), sensor response and leakage as reasons real records differ from the reversible model. [John Hart, University of Colorado (2000), Adiabatic Expansion and Gas Law Physics: sensor demonstration and limitations](https://atoc.colorado.edu/TeachingandLearning/Demonstrations/AdiabaticExpansion/Adiabatic_expansion.htm)

For a proposed rapid-versus-slow comparison, let the air and walls return to the same initial [thermal equilibrium](thermal-equilibrium.md) before each run, then compare the same starting and finishing [volume](volume-thermodynamics.md) values with different stroke durations. Read [temperature](temperature.md), absolute [pressure](pressure.md) and position continuously, including the hold after motion stops. A rapid compression gives a temporary [temperature](temperature.md) rise; holding the smaller [volume](volume-thermodynamics.md) lets [heat](heat.md) leave and the [temperature](temperature.md) approach the surroundings again. Slow compression in good thermal contact allows that [heat transfer](heat-transfer.md) during the stroke and approaches an [isothermal compression](isothermal-compression.md). Loaded expansion reverses the signs: the rapid stroke cools, while [heat](heat.md) entering during slow motion reduces the cooling. PASCO explicitly supports rapid nearly [adiabatic processes](adiabatic-process.md) and slow [isothermal processes](isothermal-process.md); the matched-run controls here are a proposed extension, not a reported set of measurements. [PASCO scientific, TD-8565 product documentation: simultaneous readouts and adiabatic/isothermal comparisons](https://www.pasco.com/products/lab-apparatus/thermodynamics/gas-laws/td-8565)

Insulation suppresses [thermal conduction](thermal-conduction.md); it does not prove that [heat transfer](heat-transfer.md) vanishes. As proposed controls, repeat the matched strokes with and without a removable insulating jacket, record room and wall [temperatures](temperature.md), measure fixed-position drift, and check valve closure and seal leakage. Calibrate the [thermometer](thermometer.md) and position readout independently, including any connected dead [volume](volume-thermodynamics.md); account for the [heat capacity](heat-capacity.md) of the probe rather than treating it as a passive observer. Hart explicitly identifies the small air sample relative to the probe and walls, sensor inertia and seal leakage as limitations. A fast display cannot eliminate those physical effects. [John Hart, Adiabatic Expansion and Gas Law Physics: wall, probe and seal limitations](https://atoc.colorado.edu/TeachingandLearning/Demonstrations/AdiabaticExpansion/Adiabatic_expansion.htm)

There are two distinct timing requirements. Let $\tau_{\rm eq}$ describe internal equilibration, $\tau_{\rm probe}$ the [thermometer](thermometer.md) response, $t_{\rm move}$ the stroke duration and $\tau_{\rm heat}$ the effective [heat transfer](heat-transfer.md) [time constant](time-constant.md). A useful sufficient window for a resolved, nearly reversible [adiabatic process](adiabatic-process.md) is

$$
\tau_{\rm eq},\tau_{\rm probe}\ll t_{\rm move}\ll\tau_{\rm heat},
$$

with negligible [friction](friction.md). The left inequality permits a [quasistatic process](quasistatic-process.md) and a usable readout; the right limits [heat](heat.md) leakage. A violent stroke may satisfy only the right inequality. PASCO reports a roughly $30$–$50\,\mathrm{ms}$ lag of its [temperature](temperature.md) channel behind the other channels, so apparent simultaneous samples require care. If no such window exists, analyze equilibrium endpoints with the [first law of thermodynamics](first-law-of-thermodynamics.md), and regard the path as approximate. [PASCO scientific, guide 012-05110D, p. 4: temperature-sensor lag](https://cdn.pasco.com/product_document/Adiabatic-Gas-Law-Apparatus-TD-8565-Manual.pdf)

<a id="image-direct-temperature-readout-and-a-heat-transfer-time-constant-in-an-adiabatic-process-experiment"></a>
![](adiabatic-processes-sensor-and-timescales.png)

**[Figure 57](#image-direct-temperature-readout-and-a-heat-transfer-time-constant-in-an-adiabatic-process-experiment). Direct temperature readout and a heat transfer time constant in an adiabatic process experiment**. Original apparatus schematic and analytical fixed-[volume](volume-thermodynamics.md) relaxation model, not measured records. After a stroke and internal equilibration, the stipulated [Newton's law of cooling](newton-s-law-of-cooling.md) model gives $[T(t)-T_b]/|T(0)-T_b|=\pm e^{-t/\tau_{\rm heat}}$. The positive and negative curves illustrate the holds after compression and loaded expansion. The drawing is a generic sensor arrangement, not a reproduction of a commercial device; it distinguishes the small probe from the walls and their possible [heat transfer](heat-transfer.md).

The diagram's model is deliberately a hold after the stroke, when boundary [work](work.md) is zero. For constant whole-sample [heat capacity at constant volume](heat-capacity-at-constant-volume.md) $C_V$ and effective thermal conductance $K>0$, it assumes

$$
C_V\frac{dT}{dt}=-K(T-T_b),\qquad
\tau_{\rm heat}=\frac{C_V}{K},\qquad
T(t)-T_b=[T(0)-T_b]e^{-t/\tau_{\rm heat}}.
$$

This is [Newton's law of cooling](newton-s-law-of-cooling.md) with one uniform [gas](gas.md) [temperature](temperature.md) and a fixed surrounding [temperature](temperature.md); actual wall and probe dynamics can require more than one [time constant](time-constant.md). At $t/\tau_{\rm heat}=0.1$, the fraction of the initial [temperature](temperature.md) anomaly erased is $1-e^{-0.1}\simeq0.0952$; at one [time constant](time-constant.md) it is about $0.6321$. These are analytical fractions, not experimental tolerances or evidence that the preceding stroke was reversible. Measuring the hold helps estimate [heat](heat.md) leakage independently of the motion.

The usefulness of an [adiabatic process](adiabatic-process.md) is that it separates mechanical [work](work.md) from [heat transfer](heat-transfer.md). Its reversible limit connects [temperature](temperature.md) changes, mechanical stiffness and [entropy](entropy.md) in one model: [Rüchardt experiment](ruchardt-experiment.md) and [Clément-Desormes experiment](clement-desormes-experiment.md) already use that connection to measure [heat capacity ratio](heat-capacity-ratio.md). The contrast with [free expansion](free-expansion.md) explains the deeper point: suppressing [heat](heat.md) does not determine how much [work](work.md) is exchanged or how much [entropy](entropy.md) is produced.

**Table of contents**

- [Adiabatic compression](adiabatic-compression.md)
- [Adiabatic expansion](adiabatic-expansion.md)
- [Isentropic process](isentropic-process.md)
- [Reversible ideal-gas adiabat](reversible-ideal-gas-adiabat.md)

## ↑ Ancestors (6)

1. [First law of thermodynamics](first-law-of-thermodynamics.md)
2. [Thermodynamics](thermodynamics-split.md)
3. [Statistical physics](statistical-physics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (38)

- [Adiabatic compression](adiabatic-compression.md)
- [Adiabatic expansion](adiabatic-expansion.md)
- [Adiabatic process](adiabatic-process.md)
- [Adiabatic scaling of a Fermi gas with power-law density of states](adiabatic-scaling-of-a-fermi-gas-with-power-law-density-of-states.md)
- [Compressibility](compressibility.md)
- [Crocco form of the unsteady Euler equation](crocco-form-of-the-unsteady-euler-equation.md)
- [Dry parcel buoyancy in a homogeneous atmosphere](dry-parcel-buoyancy-in-a-homogeneous-atmosphere.md)
- [Entropy change in free expansion](entropy-change-in-free-expansion.md)
- [Entropy density of a photon gas](entropy-density-of-a-photon-gas.md)
- [First law of thermodynamics](first-law-of-thermodynamics.md)
- [Heat](heat.md)
- [Heat capacity ratio](heat-capacity-ratio.md)
- [Homologous adiabatic stellar stability](homologous-adiabatic-stellar-stability.md)
- [Isentropic compressibility](isentropic-compressibility.md)
- [Isentropic process](isentropic-process.md)
- [Isothermal process](isothermal-process.md)
- [Maxwell relations](maxwell-relations.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-62/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-63/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-70/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-71/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-63/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-58/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-310/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-315/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-314/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-314/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-315/1/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-1/35d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-1/36c/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4/35a/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4/39c/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-321/3/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-314/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-347/1/b/solution.md)
- [Reversible thermodynamic process](reversible-thermodynamic-process.md)
- [Rüchardt experiment](ruchardt-experiment.md)
- [Stellar convective instability](stellar-convective-instability.md)
