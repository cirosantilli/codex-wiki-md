# Heat capacity

↑ **Parent:** [Heat](heat.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Heat_capacity)

Heat capacity measures the [heat](heat.md) supplied per small [temperature](temperature.md) increase along a specified process:

$$
C_X=\left(\frac{\delta Q}{dT}\right)_X.
$$

The subscript $X$ records the constraint, such as fixed [volume](volume-thermodynamics.md) or fixed [pressure](pressure.md). The units are $\mathrm{J\,K^{-1}}$. The symbol $\delta Q$ emphasizes that [heat](heat.md) is a transfer along a path, rather than a [state function](state-function.md) with a differential $dQ$. Consequently, an unspecified [heat capacity](heat-capacity.md) does not determine the required [heat](heat.md).

For a [closed system](closed-system.md) of fixed composition undergoing a [quasistatic process](quasistatic-process.md), assume that only [pressure](pressure.md)-[volume](volume-thermodynamics.md) [work](work.md) occurs, with no [friction](friction.md) and no change in bulk [kinetic energy](kinetic-energy.md) or [potential energy](potential-energy.md). The [first law of thermodynamics](first-law-of-thermodynamics.md) and $H=U+pV$, where $U$ is [internal energy](internal-energy.md) and $H$ is [enthalpy](enthalpy.md), then give

$$
\delta Q=dU+p\,dV=dH-V\,dp,\qquad
C_V=\left(\frac{\partial U}{\partial T}\right)_V,\qquad
C_p=\left(\frac{\partial H}{\partial T}\right)_p.
$$

These [partial derivatives](partial-derivative.md) define [heat capacity at constant volume](heat-capacity-at-constant-volume.md) and [heat capacity at constant pressure](heat-capacity-at-constant-pressure.md), with the amount and composition also held fixed. Integrating along the selected constraint gives $Q=\int_{T_1}^{T_2}C_X(T)\,dT$ within a single [thermodynamic phase](thermodynamic-phase.md); $Q=C_X\Delta T$ requires constant $C_X$. [4 Classical Thermodynamics](statistical-physics-by-david-tong/4-classical-thermodynamics.md)

For a computed example, take a [monatomic gas](monatomic-gas.md) in the classical [ideal gas](ideal-gas.md) regime, with [amount of substance](amount-of-substance.md) $n=1\,\mathrm{mol}$ and stipulated [molar gas constant](molar-gas-constant.md) $R=8.314\,\mathrm{J\,mol^{-1}\,K^{-1}}$. The [equipartition theorem](equipartition-theorem.md) gives $U=3nRT/2$, and the [ideal gas law](ideal-gas-law.md) gives $pV=nRT$. Thus

$$
C_V=\frac32nR=12.471\,\mathrm{J\,K^{-1}},\qquad
C_p=\frac52nR=20.785\,\mathrm{J\,K^{-1}}.
$$

For the same [temperature](temperature.md) increase $\Delta T=10\,\mathrm K$, the two processes require

$$
Q_V=124.71\,\mathrm J,\qquad Q_p=207.85\,\mathrm J,\qquad
\Delta U_V=\Delta U_p=124.71\,\mathrm J,\qquad
W_V=0,\quad W_p=p\Delta V=nR\Delta T=83.14\,\mathrm J.
$$

Here [work](work.md) done by the [gas](gas.md) is positive. At fixed [pressure](pressure.md), the extra [heat](heat.md) supplies expansion [work](work.md); the [internal energy](internal-energy.md) increase is the same because [internal energy of an ideal gas](internal-energy-of-an-ideal-gas.md) depends only on [temperature](temperature.md). Their final [volume](volume-thermodynamics.md) values differ. [OpenStax, Heat capacities of an ideal gas](https://openstax.org/books/university-physics-volume-2/pages/3-5-heat-capacities-of-an-ideal-gas)

<a id="image-required-heat-depends-on-the-constraint-and-the-amount-of-material"></a>
![](heat-capacity-constraints.png)

**[Figure 37](#image-required-heat-depends-on-the-constraint-and-the-amount-of-material). Required heat depends on the constraint and the amount of material**. Left: one [mole](mole-unit.md) of classical [monatomic gas](monatomic-gas.md) with the stipulated [molar gas constant](molar-gas-constant.md) above; the shaded difference is expansion [work](work.md) at fixed [pressure](pressure.md). Right: the illustrative fixed-[volume](volume-thermodynamics.md) body from [specific heat capacity](specific-heat-capacity.md), with [mass](mass.md) $2\,\mathrm{kg}$ and $c_V=400\,\mathrm{J\,kg^{-1}\,K^{-1}}$. Each curve starts at zero accumulated [heat](heat.md), rather than zero absolute [internal energy](internal-energy.md).

The practical value of [heat capacity](heat-capacity.md) is that a measured [heat](heat.md) input and [temperature](temperature.md) response can determine it. Once its constraint and [temperature](temperature.md) dependence are known, it predicts heating requirements and supplies [entropy](entropy.md) changes through [entropy from heat capacity](entropy-from-heat-capacity.md). [Tong, Statistical Physics, heat capacity as a measurable response](https://davidtong.org/teaching/statistical-physics/statmechhtml/S1)

**Table of contents**

- [Molar heat capacity](molar-heat-capacity.md)
- [Heating curve](heating-curve.md)
- [Entropy from heat capacity](entropy-from-heat-capacity.md)
- [Entropy concavity and positive heat capacity](entropy-concavity-and-positive-heat-capacity.md)
- [Specific heat capacity](specific-heat-capacity.md)
  - [Volumetric heat capacity](volumetric-heat-capacity.md)
  - [Specific heat capacity at constant volume](specific-heat-capacity-at-constant-volume.md)
  - [Specific heat capacity at constant pressure](specific-heat-capacity-at-constant-pressure.md)
    - [Pure-radiation constant-pressure heat-capacity singularity](pure-radiation-constant-pressure-heat-capacity-singularity.md)
- [Heat capacity at constant volume](heat-capacity-at-constant-volume.md)
  - [Dulong-Petit law](dulong-petit-law.md)
    - [Einstein solid](einstein-solid.md)
- [Heat capacity at constant area](heat-capacity-at-constant-area.md)

## ↑ Ancestors (6)

1. [Heat](heat.md)
2. [Thermodynamics](thermodynamics-split.md)
3. [Statistical physics](statistical-physics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (103)

- [Adiabatic process](adiabatic-process.md)
- [Advection-driven melting front in a porous matrix](advection-driven-melting-front-in-a-porous-matrix.md)
- [Boundary-pressure correction to the virial theorem](boundary-pressure-correction-to-the-virial-theorem.md)
- [Calorimeter](calorimeter.md)
- [Calorimeter calibration](calorimeter-calibration.md)
- [Calorimeter heat-loss correction](calorimeter-heat-loss-correction.md)
- [Calorimetry](calorimetry.md)
- [Canonical partition function](canonical-partition-function.md)
- [Carnot's theorem](carnot-s-theorem.md)
- [Coefficient of thermal expansion](coefficient-of-thermal-expansion.md)
- [Dulong-Petit law](dulong-petit-law.md)
- [Einstein solid](einstein-solid.md)
- [Electrical calorimetry of a resistor](electrical-calorimetry-of-a-resistor.md)
- [Entropy](entropy.md)
- [Entropy concavity and positive heat capacity](entropy-concavity-and-positive-heat-capacity.md)
- [Entropy density of a photon gas](entropy-density-of-a-photon-gas.md)
- [Entropy maximization under thermal contact](entropy-maximization-under-thermal-contact.md)
- [Equipartition theorem](equipartition-theorem.md)
- [Finite-rate isothermal piston model](finite-rate-isothermal-piston-model.md)
- [Free expansion](free-expansion.md)
- [Gaussian specific-heat infrared threshold](gaussian-specific-heat-infrared-threshold.md)
- [Gibbs free energy](gibbs-free-energy.md)
- [Heat capacity](heat-capacity.md)
- [Heat capacity at constant pressure](heat-capacity-at-constant-pressure.md)
- [Heat capacity at constant volume](heat-capacity-at-constant-volume.md)
- [Heat-engine calorimetry](heat-engine-calorimetry.md)
- [Heat-pump calorimetry](heat-pump-calorimetry.md)
- [Heating curve](heating-curve.md)
- [Ice-melting calorimetry](ice-melting-calorimetry.md)
- [Ideal gas](ideal-gas.md)
- [Ideal gas law](ideal-gas-law.md)
- [Infrared](infrared.md)
- [Internal energy of an ideal gas](internal-energy-of-an-ideal-gas.md)
- [Joule's free-expansion experiment](joule-s-free-expansion-experiment.md)
- [Joule's paddle-wheel experiment](joule-s-paddle-wheel-experiment.md)
- [Large-concentration stagnant-mush similarity](large-concentration-stagnant-mush-similarity.md)
- [Laser flash analysis](laser-flash-analysis.md)
- [Latent heat](latent-heat.md)
- [Lattice enthalpy from solution calorimetry](lattice-enthalpy-from-solution-calorimetry.md)
- [Linear thermoelasticity with prescribed thermal volume](linear-thermoelasticity-with-prescribed-thermal-volume.md)
- [Maxwell relations](maxwell-relations.md)
- [Mayer's relation](mayer-s-relation.md)
- [Mixing calorimetry](mixing-calorimetry.md)
- [Molar heat capacity](molar-heat-capacity.md)
- [Negative heat capacity of a Schwarzschild black hole](negative-heat-capacity-of-a-schwarzschild-black-hole.md)
- [Negative heat capacity of a virialized gravitational system](negative-heat-capacity-of-a-virialized-gravitational-system.md)
- [Paddle-wheel calorimetry energy balance](paddle-wheel-calorimetry-energy-balance.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-52/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-64/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-64/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-69/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-69/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-57/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-75/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-4/34d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-51/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-51/3/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-51/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-2/34d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-76/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-83/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-83/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-69/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-2/35d/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-62/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-62/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-41/1/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-49/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-49/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-65/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-55/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-78/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-332/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-303/1/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-321/1/b/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-3/36a/b/v/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-303/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-303/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-311/4/c/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-311/4/d/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-4/35b/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-303/1/a/ii/solution.md)
- [Quasistatic process](quasistatic-process.md)
- [Sensible heat](sensible-heat.md)
- [Specific heat capacity](specific-heat-capacity.md)
- [Specific heat capacity at constant pressure](specific-heat-capacity-at-constant-pressure.md)
- [Statistical mechanics](statistical-mechanics.md)
- [Statistical physics](statistical-physics-split.md)
- [Temperature](temperature.md)
- [Temperature sensitivity of a free-expansion experiment](temperature-sensitivity-of-a-free-expansion-experiment.md)
- [Thermal diffusion rate of a Fourier mode](thermal-diffusion-rate-of-a-fourier-mode.md)
- [Thermal diffusivity](thermal-diffusivity.md)
- [Thermal equilibration of two finite bodies](thermal-equilibration-of-two-finite-bodies.md)
- [Thermal equilibrium](thermal-equilibrium.md)
- [Thermal inertia](thermal-inertia.md)
- [Thermal instability from negative hydrogen ion opacity](thermal-instability-from-negative-hydrogen-ion-opacity.md)
- [Thermometer](thermometer.md)
- [Universal specific-heat amplitude ratio](universal-specific-heat-amplitude-ratio.md)
- [Virial theorem for a homogeneous pair potential](virial-theorem-for-a-homogeneous-pair-potential.md)
- [Volumetric heat capacity](volumetric-heat-capacity.md)
- [Zero-dimensional planetary energy balance](zero-dimensional-planetary-energy-balance.md)
- [Zeroth law of thermodynamics](zeroth-law-of-thermodynamics.md)
- [Zeroth-law thermometer comparison](zeroth-law-thermometer-comparison.md)
