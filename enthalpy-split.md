# Enthalpy

↑ **Parent:** [Thermodynamics](thermodynamics-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Enthalpy)

Enthalpy is the [state function](state-function.md) obtained by adding [pressure](pressure-split.md) times [volume](volume-thermodynamics.md) to [internal energy](internal-energy-split.md):

$$
H=U+pV.
$$

Here $U$ denotes [internal energy](internal-energy-split.md), also written $E$ in some references. Like [internal energy](internal-energy-split.md), [enthalpy](enthalpy-split.md) is measured in [joules](joule.md) and is an [extensive variable](extensive-quantity.md). Its definition packages the [internal energy](internal-energy-split.md) change and expansion [work](work.md) into one useful quantity for fixed-[pressure](pressure-split.md) calculations. It does not define a body's stored [heat](heat-split.md). [IUPAC Gold Book, enthalpy](https://goldbook.iupac.org/terms/view/E02141/plain)

For a fixed amount and composition of a [simple compressible system](simple-compressible-system.md), the relation between neighboring equilibrium states is

$$
dH=T\,dS+V\,dp.
$$

Here $T$ is absolute [temperature](temperature-split.md) and $S$ is [entropy](entropy-split.md). Thus [entropy](entropy-split.md) and [pressure](pressure-split.md) are the natural variables of this [thermodynamic potential](thermodynamic-potential-split.md), with [partial derivatives](partial-derivative.md) $T=(\partial H/\partial S)_p$ and $V=(\partial H/\partial p)_S$. Fixed composition matters: changing composition adds further terms. The formula follows in one line from the equilibrium [first law of thermodynamics](first-law-of-thermodynamics-split.md) identity:

$$
dH=dU+p\,dV+V\,dp=(T\,dS-p\,dV)+p\,dV+V\,dp=T\,dS+V\,dp.
$$

The cancellation of $p\,dV$ is the reason [enthalpy](enthalpy-split.md) replaces [volume](volume-thermodynamics.md) with [pressure](pressure-split.md) as a natural variable. This identity concerns equilibrium states; it does not identify $T\,dS$ with actual irreversible [heat](heat-split.md) transfer. [David Tong, Statistical Physics, section 4.4.1: enthalpy](https://davidtong.org/teaching/statistical-physics/statmechhtml/S4#S4.SS4.SSS1)

For a [closed system](closed-system.md) undergoing a [quasistatic process](quasistatic-process.md) at constant [pressure](pressure-split.md), require fixed amount and composition, only [pressure](pressure-split.md)-[volume](volume-thermodynamics.md) [work](work.md), no [friction](friction.md), and unchanged bulk [kinetic energy](kinetic-energy.md) and [potential energy](potential-energy.md). Then the actual [first law of thermodynamics](first-law-of-thermodynamics-split.md) balance gives

$$
\delta Q=dU+p\,dV=dH-V\,dp,\qquad
dp=0\ \Longrightarrow\ Q_p=\Delta H.
$$

The symbol $Q_p$ means transferred [heat](heat-split.md) for this fixed-[pressure](pressure-split.md) process. If the piston example in [heat](heat-split.md) additionally meets these conditions, its $20\,\mathrm{kJ}$ of incoming [heat](heat-split.md) equals $\Delta H$, while $\Delta U=15\,\mathrm{kJ}$ and $p\Delta V=W=5\,\mathrm{kJ}$. The example shows exactly what [enthalpy](enthalpy-split.md) adds to [internal energy](internal-energy-split.md): the expansion [work](work.md) required at the imposed [pressure](pressure-split.md).

Within a single [thermodynamic phase](thermodynamic-phase.md), [heat capacity at constant pressure](heat-capacity-at-constant-pressure.md) gives

$$
C_p=\left(\frac{\partial H}{\partial T}\right)_p,\qquad
\Delta H=\int_{T_1}^{T_2}C_p(T)\,dT
$$

with the amount and composition fixed. Constant $C_p$ gives $\Delta H=C_p\Delta T$; dividing by [mass](mass.md) gives [specific heat capacity at constant pressure](specific-heat-capacity-at-constant-pressure.md). At equilibrium [melting](melting.md), [enthalpy](enthalpy-split.md) can instead change through [latent heat](latent-heat.md) while [temperature](temperature-split.md) stays fixed. The [sensible heat](sensible-heat.md) example therefore adds two single-[thermodynamic phase](thermodynamic-phase.md) [enthalpy](enthalpy-split.md) changes and one [latent heat](latent-heat.md) contribution.

The usefulness of [enthalpy](enthalpy-split.md) lies in matching the imposed constraint: a fixed-[pressure](pressure-split.md) experiment naturally reports $\Delta H$, while fixed-[volume](volume-thermodynamics.md) heating with no other [work](work.md) reports $\Delta U$. Neither equality is universal. Additional [work](work.md) or changing [pressure](pressure-split.md) alters the relation between supplied [heat](heat-split.md) and $\Delta H$; irreversible [entropy](entropy-split.md) production also prevents identifying actual $\delta Q$ with $T\,dS$. The separate [Joule-Thomson coefficient](joule-thomson-coefficient.md) branch uses [enthalpy](enthalpy-split.md) to describe throttling under its own assumptions.

**Table of contents**

- [Stagnation enthalpy](stagnation-enthalpy.md)
- [Enthalpy of mixing](enthalpy-of-mixing.md)
- [Reaction enthalpy](reaction-enthalpy.md)
- [Molar enthalpy](molar-enthalpy.md)
- [Isenthalpic process](isenthalpic-process.md)
- [Steady-flow energy balance](steady-flow-energy-balance.md)
- [Joule-Thomson effect](joule-thomson-effect.md)
  - [Measuring the Joule-Thomson effect with a porous plug](measuring-the-joule-thomson-effect-with-a-porous-plug.md)
- [Joule-Thomson coefficient](joule-thomson-coefficient.md)
  - [Joule-Thomson inversion curve](joule-thomson-inversion-curve.md)
    - [Joule-Thomson inversion temperature](joule-thomson-inversion-temperature.md)
  - [Van der Waals throttling model](van-der-waals-throttling-model.md)
  - [Virial criterion for Joule-Thomson cooling](virial-criterion-for-joule-thomson-cooling.md)
- [Specific enthalpy](specific-enthalpy.md)
  - [Polytropic enthalpy](polytropic-enthalpy.md)
- [Enthalpy Maxwell relation](enthalpy-maxwell-relation.md)
- [Heat capacity at constant pressure](heat-capacity-at-constant-pressure.md)
  - [Difference between constant-pressure and constant-volume heat capacities](difference-between-constant-pressure-and-constant-volume-heat-capacities.md)
    - [Heat-capacity difference and mechanical stability](heat-capacity-difference-and-mechanical-stability.md)
    - [Volume derivative form of the heat-capacity difference](volume-derivative-form-of-the-heat-capacity-difference.md)

## ↑ Ancestors (5)

1. [Thermodynamics](thermodynamics-split.md)
2. [Statistical physics](statistical-physics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (126)

- [Activation energy](activation-energy.md)
- [Advection-driven melting front in a porous matrix](advection-driven-melting-front-in-a-porous-matrix.md)
- [Bond-dissociation energy](bond-dissociation-energy.md)
- [Bond-dissociation enthalpy](bond-dissociation-enthalpy.md)
- [Born-Haber cycle](born-haber-cycle.md)
- [Calorimeter calibration](calorimeter-calibration.md)
- [Calorimetry](calorimetry-split.md)
- [Clausius-Clapeyron relation](clausius-clapeyron-relation.md)
- [Desolvation](desolvation.md)
- [Electrical calorimetry of a resistor](electrical-calorimetry-of-a-resistor.md)
- [Electron attachment enthalpy](electron-attachment-enthalpy.md)
- [Energy profile (chemistry)](energy-profile-chemistry.md)
- [Enthalpy](enthalpy-split.md)
- [Enthalpy change of solution](enthalpy-change-of-solution.md)
- [Enthalpy cycle](enthalpy-cycle.md)
- [Enthalpy of activation](enthalpy-of-activation.md)
- [Enthalpy of atomization](enthalpy-of-atomization.md)
- [Enthalpy of vaporization](enthalpy-of-vaporization.md)
- [Entropy generation by mixing equal thermal masses](entropy-generation-by-mixing-equal-thermal-masses.md)
- [Frazil export enthalpy balance](frazil-export-enthalpy-balance.md)
- [Free expansion](free-expansion.md)
- [Gibbs free energy](gibbs-free-energy.md)
- [Gibbs free energy of mixing](gibbs-free-energy-of-mixing.md)
- [Heat](heat-split.md)
- [Heat capacity](heat-capacity.md)
- [Heat capacity at constant pressure](heat-capacity-at-constant-pressure.md)
- [Helium liquefaction](helium-liquefaction.md)
- [Hess's law](hess-s-law.md)
- [Hess's law calorimetry experiment](hess-s-law-calorimetry-experiment.md)
- [Hess's law equation cancellation](hess-s-law-equation-cancellation.md)
- [Hydration enthalpy](hydration-enthalpy.md)
- [Hydrophobic effect](hydrophobic-effect.md)
- [Ice-melting calorimetry](ice-melting-calorimetry.md)
- [Internal energy at constant temperature](internal-energy-at-constant-temperature.md)
- [Isenthalpic process](isenthalpic-process.md)
- [James Prescott Joule](james-prescott-joule.md)
- [Joule-Thomson coefficient](joule-thomson-coefficient.md)
- [Joule-Thomson effect](joule-thomson-effect.md)
- [Kirchhoff's law of thermochemistry](kirchhoff-s-law-of-thermochemistry.md)
- [Latent heat](latent-heat.md)
- [Latent heat of fusion](latent-heat-of-fusion.md)
- [Lattice energy](lattice-energy.md)
- [Lattice enthalpy from solution calorimetry](lattice-enthalpy-from-solution-calorimetry.md)
- [Liquefaction enthalpy budget](liquefaction-enthalpy-budget.md)
- [Maxwell relations](maxwell-relations.md)
- [Mayer's relation](mayer-s-relation.md)
- [Melting-front instability due to permeability contrast](melting-front-instability-due-to-permeability-contrast.md)
- [Melting pressure inferred from flotation and latent heats](melting-pressure-inferred-from-flotation-and-latent-heats.md)
- [Mixing calorimetry](mixing-calorimetry.md)
- [Molar enthalpy](molar-enthalpy.md)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2012/paper-1/2/a/solution.md)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2012/paper-1/2/c/solution.md)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2017/3/b/solution.md)
- [Solution](past-exam-of-the-chemistry-b-course-of-the-university-of-cambridge/2022/paper-1/b5/a/iii/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1/4/a/iii/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1/4/a/vi/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1/4/b/i/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1/4/b/ii/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1/5/c/iii/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1/6/a/iii/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1/6/a/iv/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-1/2/a/v/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-1/4/a/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-1/4/b/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-1/5/c/v/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1/10/b/ii/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1/10/b/iii/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-3/47/a/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-3/47/b/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-3/47/c/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-id/2/a/solution.md)
- [Solution](past-exam-of-the-formation-of-structure-in-the-universe-course-of-the-university-of-cambridge/2012/paper-1/1/c/solution.md)
- [Solution](past-exam-of-the-formation-of-structure-in-the-universe-course-of-the-university-of-cambridge/2014/paper-1/3/a/solution.md)
- [Solution](past-exam-of-the-materials-science-course-of-the-university-of-cambridge/2015/paper-1/4/a/solution.md)
- [Solution](past-exam-of-the-materials-science-course-of-the-university-of-cambridge/2016/paper-1/6/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-35/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-77/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-4/34d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-70/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-71/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-2/34d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-65/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-65/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-89/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-3/35c/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-80/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-3/33c/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-315/2/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-314/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-332/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-332/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ii/paper-2/37c/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-4/39c/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-314/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2003/paper-2/9/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-2/17/a/solution.md)
- [Solution](past-exam-of-the-mphil-in-micro-and-nanotechnology-enterprise-course-of-the-university-of-cambridge/2017/paper-1/section-a-iii/6/ii/solution.md)
- [Solution](past-exam-of-the-mphil-in-micro-and-nanotechnology-enterprise-course-of-the-university-of-cambridge/2021/paper-1/10/i/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2011/paper-1/section-c/c10/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2012/paper-2/section-c/c10/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2012/paper-2/section-c/c13/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2013/paper-2/section-c/c11/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2017/paper-2/section-c/c11/b/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2018/paper-2/section-c/c13/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2022/paper-2/section-a/a4/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2022/paper-2/section-c/c8/e/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-1/section-b/b3/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-1/b1/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2004/section-b/b7/a/solution.md)
- [Solution](past-exam-of-the-relativistic-astrophysics-and-cosmology-course-of-the-university-of-cambridge/2013/paper-1/3/d/solution.md)
- [Solution](past-exam-of-the-relativistic-astrophysics-and-cosmology-course-of-the-university-of-cambridge/2014/paper-1/3/c/solution.md)
- [Phase diagram](phase-diagram.md)
- [Physical properties of salts](physical-properties-of-salts.md)
- [Polytropic enthalpy](polytropic-enthalpy.md)
- [Reaction enthalpy](reaction-enthalpy.md)
- [Sensible heat](sensible-heat.md)
- [Sequential bond-dissociation energies](sequential-bond-dissociation-energies.md)
- [Solubility](solubility.md)
- [Solvation thermodynamic balance](solvation-thermodynamic-balance.md)
- [Specific enthalpy](specific-enthalpy.md)
- [Stagnation enthalpy](stagnation-enthalpy.md)
- [Standard enthalpy of formation](standard-enthalpy-of-formation.md)
- [State function](state-function.md)
- [Thermodynamic potential](thermodynamic-potential-split.md)
- [Two reversible ideal-gas paths between the same states](two-reversible-ideal-gas-paths-between-the-same-states.md)
- [Volume derivative form of the heat-capacity difference](volume-derivative-form-of-the-heat-capacity-difference.md)
