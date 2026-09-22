# Canonical partition function

↑ **Parent:** [Canonical ensemble](canonical-ensemble-split.md)

The [partition function](canonical-partition-function.md) $Z(\beta)=\sum_s e^{-\beta E_s}$ is the sum of the [Boltzmann weights](boltzmann-factor.md) over individual [microstates](microstate.md). Dividing by it makes their [probabilities](probability.md) sum to one. When summing distinct [energies](energy-split.md) instead, include the [state degeneracy](state-degeneracy.md): $Z=\sum_E g(E)e^{-\beta E}$. For two independent distinguishable [two-level systems](two-level-system.md),

$$
Z_2=1+2e^{-\beta\Delta}+e^{-2\beta\Delta}=Z_1^2.
$$

The middle coefficient counts two [microstates](microstate.md), exactly as in the preceding figure. For $N$ such units, $Z_N=Z_1^N$; this factorization requires additive [energy](energy-split.md) and [independence](independent-random-variables.md), and generally fails with interactions.

The usefulness goes beyond normalization. For fixed [energies](energy-split.md), [derivatives](derivative.md) of the [natural logarithm](natural-logarithm.md) of the [partition function](canonical-partition-function.md) yield measurable quantities:

$$
U=\langle E\rangle=-\partial_\beta\ln Z,\qquad
\operatorname{Var}(E)=\partial_\beta^2\ln Z,\qquad
S=k_B(\ln Z+\beta U).
$$

Here $U$ is [internal energy](internal-energy-split.md), the second expression is the [energy](energy-split.md) [variance](variance-split.md), and $S$ is [Gibbs entropy](gibbs-entropy.md). For one [two-level system](two-level-system.md) at fixed $\Delta$, its [heat capacity](heat-capacity.md) $C=\partial U/\partial T$ and [entropy](entropy-split.md) are

$$
U=\Delta p,\qquad \frac{C}{k_B}=\frac{(\beta\Delta)^2e^{\beta\Delta}}{(1+e^{\beta\Delta})^2},\qquad
\frac{S}{k_B}=\ln(1+e^{-\beta\Delta})+\beta\Delta p.
$$

At $\beta\Delta=\ln3$, these give $U/\Delta=0.25$, $C/k_B\simeq0.2263$ and $S/k_B\simeq0.5623$. For independent units, all three quantities add.

The figure shows why [heat capacity](heat-capacity.md) peaks. At low [temperature](temperature-split.md), the excited [energy](energy-split.md) is rarely occupied; at high [temperature](temperature-split.md), the [probabilities](probability.md) are almost equal and further warming barely changes [internal energy](internal-energy-split.md). The largest response lies between these limits, at $k_BT/\Delta\simeq0.4168$, where $C/k_B\simeq0.4392$. Meanwhile [entropy](entropy-split.md) rises from zero toward $k_B\ln2$, reflecting two equally likely alternatives. This high-[temperature](temperature-split.md) limit belongs to the stipulated [two-level system](two-level-system.md); extra accessible [energy eigenstates](energy-eigenstate.md) would change it.

<a id="image-population-heat-capacity-and-entropy-of-one-two-level-system-as-temperature-increases"></a>
![](two-level-thermal-response.png)

**[Figure 1](#image-population-heat-capacity-and-entropy-of-one-two-level-system-as-temperature-increases). Population, heat capacity and entropy of one two-level system as temperature increases**.

**Table of contents**

- [Gibbs paradox](gibbs-paradox.md)
- [Molecular partition function](molecular-partition-function.md)
  - [Energy reference in molecular partition functions](energy-reference-in-molecular-partition-functions.md)
  - [Molecular partition function density](molecular-partition-function-density.md)
- [Electronic partition function](electronic-partition-function.md)
- [Vibrational partition function](vibrational-partition-function.md)
  - [Vibrational entropy](vibrational-entropy.md)
- [Rotational partition function](rotational-partition-function.md)
  - [Rotational entropy](rotational-entropy.md)
- [Translational partition function](translational-partition-function.md)
- [Thermal trace](thermal-trace.md)
  - [Parity-twisted oscillator thermal trace](parity-twisted-oscillator-thermal-trace.md)
- [Thermodynamic derivatives of the canonical partition function](thermodynamic-derivatives-of-the-canonical-partition-function.md)
  - [Canonical energy fluctuation](canonical-energy-fluctuation.md)
    - [Relative energy fluctuation of a monatomic ideal gas](relative-energy-fluctuation-of-a-monatomic-ideal-gas.md)
- [Particle in a finite two-dimensional harmonic trap](particle-in-a-finite-two-dimensional-harmonic-trap.md)
  - [Hard-wall correction to harmonic equipartition](hard-wall-correction-to-harmonic-equipartition.md)
- [Classical ideal-gas partition function](classical-ideal-gas-partition-function.md)
  - [Classical ideal gas in a spherical linear trap](classical-ideal-gas-in-a-spherical-linear-trap.md)
    - [Quantum degeneracy threshold in a spherical linear trap](quantum-degeneracy-threshold-in-a-spherical-linear-trap.md)
    - [Isentropic decompression of a spherical linear trap](isentropic-decompression-of-a-spherical-linear-trap.md)
  - [Classical ideal gas in a homogeneous soft trap](classical-ideal-gas-in-a-homogeneous-soft-trap.md)
  - [Thermal de Broglie wavelength](thermal-de-broglie-wavelength.md)
    - [Degeneracy onset from thermal wavelength](degeneracy-onset-from-thermal-wavelength.md)
    - [Quantum concentration](quantum-concentration.md)
  - [Canonical partition function for an ultrarelativistic gas in a power-law trap](canonical-partition-function-for-an-ultrarelativistic-gas-in-a-power-law-trap.md)
    - [Most likely radius in an isotropic power-law trap](most-likely-radius-in-an-isotropic-power-law-trap.md)
  - [Sackur-Tetrode equation](sackur-tetrode-equation.md)

## ↑ Ancestors (5)

1. [Canonical ensemble](canonical-ensemble-split.md)
2. [Statistical physics](statistical-physics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (55)

- [Canonical energy variance](canonical-energy-variance.md)
- [Cluster expansion](cluster-expansion.md)
- [Einstein solid](einstein-solid.md)
- [Entropy of a two-species classical ideal gas](entropy-of-a-two-species-classical-ideal-gas.md)
- [Equal-degeneracy two-level energy and heat capacity](equal-degeneracy-two-level-energy-and-heat-capacity.md)
- [Euclidean worldline path integral](euclidean-worldline-path-integral.md)
- [Finite canonical partition function at the bosonic Hagedorn threshold](finite-canonical-partition-function-at-the-bosonic-hagedorn-threshold.md)
- [Finite-system analyticity](finite-system-analyticity.md)
- [Force-extension of a three-dimensional freely jointed chain](force-extension-of-a-three-dimensional-freely-jointed-chain.md)
- [Heat capacity of a classical magnetic dipole](heat-capacity-of-a-classical-magnetic-dipole.md)
- [Ideal chain](ideal-chain.md)
- [Isothermal-isobaric partition function](isothermal-isobaric-partition-function.md)
- [Mayer f-function](mayer-f-function.md)
- [Noninteracting subsystems](noninteracting-subsystems.md)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2021/paper-2/a6/b/solution.md)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2021/paper-2/a7/b/solution.md)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2024/paper-2/a6/a/solution.md)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2025/paper-2/a7/a/i/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-3/48/c/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-3/48/e/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-2/section-e/26/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-50/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-71/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-54/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-2/34d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-83/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-67/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-1/33c/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-4/32c/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-81/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-4/35a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-2/37a/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-2/37a/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-1/36a/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ii/paper-1/36c/a/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2014/paper-1/section-c/c10/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2018/paper-1/section-c/c11/b/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2021/paper-2/section-c/c9/a/solution.md)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2017/4/solution.md)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2018/section-a/a1/c/solution.md)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2019/section-b/4/solution.md)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2021/section-a/2/solution.md)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2021/section-b/4/a/solution.md)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2021/section-b/4/b/solution.md)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2021/section-b/5/b/solution.md)
- [Quantum Gibbs state](quantum-gibbs-state.md)
- [Rotational partition functions of hydrogen](rotational-partition-functions-of-hydrogen.md)
- [Rotational temperature](rotational-temperature.md)
- [Thermal partition function of a quantum harmonic oscillator](thermal-partition-function-of-a-quantum-harmonic-oscillator.md)
- [Thermal trace](thermal-trace.md)
- [Thermodynamic limit](thermodynamic-limit.md)
- [Translational and two-level energy variance](translational-and-two-level-energy-variance.md)
- [Translational partition function](translational-partition-function.md)
- [Vibrational heat capacity of a diatomic gas](vibrational-heat-capacity-of-a-diatomic-gas.md)
- [Virial expansion](virial-expansion.md)
