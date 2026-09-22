# Heat capacity ratio

↑ **Parent:** [Ideal gas](ideal-gas-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Heat_capacity_ratio)

The heat capacity ratio compares [heat capacity at constant pressure](heat-capacity-at-constant-pressure.md) $C_p$ with [heat capacity at constant volume](heat-capacity-at-constant-volume.md) $C_V$ at the same equilibrium state and fixed composition:

$$
\gamma=\frac{C_p}{C_V}
=\frac{C_{p,\mathrm m}}{C_{V,\mathrm m}}
=\frac{c_p}{c_V}.
$$

Here $C_p,C_V$ refer to the whole sample, in $\mathrm{J\,K^{-1}}$; [molar heat capacities](molar-heat-capacity.md) $C_{p,\mathrm m}=C_p/n$ and $C_{V,\mathrm m}=C_V/n$ are per [mole](mole-unit.md); [specific heat capacities](specific-heat-capacity.md) $c_p=C_p/m$ and $c_V=C_V/m$ are per unit [mass](mass.md). The [amount of substance](amount-of-substance.md) $n$ or [mass](mass.md) $m$ cancels only when both capacities use the same normalization. Thus [heat capacity ratio](heat-capacity-ratio.md) is dimensionless and independent of sample size. For a fixed-composition [ideal gas](ideal-gas-split.md) with positive finite $C_V$, [Mayer's relation](mayer-s-relation.md) gives

$$
\gamma(T)=1+\frac{nR}{C_V(T)}=1+\frac{R}{C_{V,\mathrm m}(T)}>1,
$$

where $R$ is the [molar gas constant](molar-gas-constant.md). More ways to store [internal energy](internal-energy-split.md) make a given [temperature](temperature-split.md) increase require more [heat](heat-split.md), bringing [heat capacity ratio](heat-capacity-ratio.md) closer to unity. [MIT Unified Engineering, Specific heats: definitions and ideal-gas relations](https://web.mit.edu/16.unified/www/FALL/thermodynamics/notes/node18.html)

The [equipartition theorem](equipartition-theorem.md) predicts $C_{V,\mathrm m}=fR/2$ when $f$ independent quadratic terms in molecular [energy](energy-split.md) are thermally active and their number stays fixed; consequently $\gamma=1+2/f$. A classical [monatomic gas](monatomic-gas.md) with no appreciable electronic excitation has $f=3$, giving $C_{V,\mathrm m}=3R/2$ and $\gamma=5/3$. For an [ideal gas](ideal-gas-split.md) of diatomic [molecules](molecule-split.md) with three translational and two rotational terms active, but its vibrational [normal mode](normal-mode.md) effectively frozen, $f=5$ gives $C_{V,\mathrm m}=5R/2$ and $\gamma=7/5$. A fully classical harmonic vibration adds both [kinetic energy](kinetic-energy.md) and [potential energy](potential-energy.md), giving $f=7$ and $\gamma=9/7$. These are model regimes, not universal constants of every [gas](gas.md): rotational freezing, electronic excitation, and changing composition invalidate the simple count.[§§2.2.1 and 2.4: equipartition and diatomic gases](statistical-physics-by-david-tong/2-classical-gases.md)

The mechanical significance of [heat capacity ratio](heat-capacity-ratio.md) follows from the [first law of thermodynamics](first-law-of-thermodynamics-split.md). For a fixed amount of [ideal gas](ideal-gas-split.md) in a reversible [adiabatic process](adiabatic-process.md), $C_V(T)\,dT=-p\,dV$. Combining this with the [ideal gas law](ideal-gas-law.md) gives the local relation

$$
\left(\frac{\partial\ln p}{\partial\ln V}\right)_S=-\gamma(T),\qquad
\int_{T_1}^{T_2}\frac{C_V(T)}{T}\,dT+nR\ln\frac{V_2}{V_1}=0.
$$

The [partial derivative](partial-derivative.md) holds at fixed [entropy](entropy-split.md) and composition even when [heat capacity ratio](heat-capacity-ratio.md) varies with [temperature](temperature-split.md). The finite-path formulas $pV^\gamma=\mathrm{constant}$ and $TV^{\gamma-1}=\mathrm{constant}$ require the additional approximation of constant [heat capacity ratio](heat-capacity-ratio.md). A rapid compression also needs internal equilibration to approximate this path; rapid motion alone does not ensure reversibility. The same local response gives [isentropic compressibility](isentropic-compressibility.md) $1/(\gamma p)$ and, for small sound disturbances in this [ideal gas](ideal-gas-split.md) regime, [speed of sound](speed-of-sound.md) $a=\sqrt{\gamma p/\rho}$, where $\rho$ is [mass density](density.md). Thus thermal storage controls mechanical stiffness, sound propagation and the measurements in [Rüchardt experiment](ruchardt-experiment.md) and [Clément-Desormes experiment](clement-desormes-experiment.md).

**Table of contents**

- [Rüchardt experiment](ruchardt-experiment.md)
- [Clément-Desormes experiment](clement-desormes-experiment.md)

## ↑ Ancestors (6)

1. [Ideal gas](ideal-gas-split.md)
2. [Thermodynamics](thermodynamics-split.md)
3. [Statistical physics](statistical-physics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (19)

- [Adiabatic compression](adiabatic-compression.md)
- [Adiabatic process](adiabatic-process.md)
- [Atmospheric blast-wave range](atmospheric-blast-wave-range.md)
- [Brayton cycle](brayton-cycle.md)
- [Clément-Desormes experiment](clement-desormes-experiment.md)
- [Cloud-chamber expansion model](cloud-chamber-expansion-model.md)
- [Compressibility](compressibility.md)
- [Heat capacity ratio](heat-capacity-ratio.md)
- [Internal energy of an ideal gas](internal-energy-of-an-ideal-gas.md)
- [Isentropic compressibility](isentropic-compressibility.md)
- [Isobaric ideal-gas internal-energy density](isobaric-ideal-gas-internal-energy-density.md)
- [Mayer's relation](mayer-s-relation.md)
- [Normal shock tables](normal-shock-tables.md)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2019/section-b/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-63/1/a/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2019/paper-1/section-a/a5/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2021/paper-1/section-a/a5/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2022/paper-2/section-c/c8/d/solution.md)
- [Rüchardt experiment](ruchardt-experiment.md)
