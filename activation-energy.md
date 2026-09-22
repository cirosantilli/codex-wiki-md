# Activation energy

↑ **Parent:** [Chemical kinetics](chemical-kinetics-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Activation_energy)

A small increase in [temperature](temperature-split.md) can produce a large increase in a [reaction rate](reaction-rate.md). In the simplest [Arrhenius equation](arrhenius-equation.md) model, warming from $300$ to $310\,\mathrm K$ increases a [rate constant](rate-constant.md) with $E_a=80\,\mathrm{kJ\,mol^{-1}}$ by about $2.81$ times, even though the absolute [thermodynamic temperature](thermodynamic-temperature.md) rises by only about $3.33\%$. This sensitivity helps explain why cooling can slow unwanted [chemical reactions](chemical-reaction-split.md) and why a hot process can become difficult to control. The comparison assumes the same [rate law](rate-law.md) and [reactant](reactant.md) [concentrations](concentration.md); the [activation energy](activation-energy.md) characterizes $k(T)$, rather than every change in the measured [reaction rate](reaction-rate.md).

The physical motivation is the distribution of molecular [energies](energy-split.md). Warming changes the [Boltzmann distribution](boltzmann-distribution.md), increasing the relative population of energetically costly configurations. A [transition state](transition-state.md) can therefore become much more accessible than the modest change in average [kinetic energy](kinetic-energy.md) might suggest. The [exponential function](exponential-function.md) in an [Arrhenius equation](arrhenius-equation.md) captures such sensitivity in a simple model; it is not a universal formula for the fraction above every barrier in a [Maxwell-Boltzmann distribution](maxwell-boltzmann-distribution.md).[§12.5, Activation Energy and the Arrhenius Equation: energy distributions and temperature sensitivity](chemistry-2e-by-paul-flowers-and-others/12-5-collision-theory.md)

[Activation energy](activation-energy.md) quantifies how strongly a [rate constant](rate-constant.md) depends on [thermodynamic temperature](thermodynamic-temperature.md). For a positive [rate constant](rate-constant.md) $k(T)$, the empirical definition is

$$
E_a(T)=RT^2\frac{d}{dT}\ln\frac{k(T)}{k_{\mathrm{ref}}},
$$

where $R$ is the [molar gas constant](molar-gas-constant.md) and $k_{\mathrm{ref}}>0$ is a fixed reference with the same units as $k$. The ratio is a [dimensionless quantity](dimensionless-quantity.md), keeping the [natural logarithm](natural-logarithm.md) meaningful without changing its [derivative](derivative.md). Thus $E_a$ is a molar [energy](energy-split.md), commonly in $\mathrm{J\,mol^{-1}}$ or $\mathrm{kJ\,mol^{-1}}$. The [Arrhenius equation](arrhenius-equation.md) makes $E_a$ constant over its assumed range. This rate-based definition, and the need for care when identifying it with a threshold on a [potential energy surface](potential-energy-surface.md), are stated in the [activation energy](iupac-compendium-of-chemical-terminology-fifth-edition-gold-book-by-international-union-of-pure-and-applied-chemistry/activation-energy.md).

In a simple barrier picture, reaching a [transition state](transition-state.md) costs [energy](energy-split.md) relative to the starting [reactants](reactant.md). The height of that barrier is different from the difference between the [reactants](reactant.md) and [reaction products](product-chemistry.md). An energetically favourable endpoint can still be reached slowly. An [energy profile](energy-profile-chemistry.md) makes the distinction visible, while an [Arrhenius plot](arrhenius-plot.md) tests temperature sensitivity from [rate constants](rate-constant.md). A measured $E_a$ need not equal a barrier read from an arbitrarily chosen diagram.

For a computed example, assume a [first-order reaction](first-order-reaction.md) has $k(300\,\mathrm K)=0.100\,\mathrm{s^{-1}}$, constant $E_a=80\,\mathrm{kJ\,mol^{-1}}$, and a temperature-independent [pre-exponential factor](pre-exponential-factor.md). The [Arrhenius equation](arrhenius-equation.md) gives

$$
\frac{k(310\,\mathrm K)}{k(300\,\mathrm K)}
=\exp\left[\frac{80000}{8.314462618}\left(\frac1{300}-\frac1{310}\right)\right]
\approx2.81398.
$$

Hence $k(310\,\mathrm K)\approx0.281398\,\mathrm{s^{-1}}$. Its [half-life](half-life.md) falls from $\ln2/0.100\approx6.93147\,\mathrm s$ to $\ln2/0.281398\approx2.46322\,\mathrm s$. These are chosen model parameters, not measurements of an identified [chemical reaction](chemical-reaction-split.md). The exponent uses [kelvin](kelvin.md), not unconverted Celsius temperatures, and $80000\,\mathrm{J\,mol^{-1}}$ must match $R$ in $\mathrm{J\,mol^{-1}\,K^{-1}}$.

<a id="image-activation-energy-potential-barriers"></a>
![](activation-energy-potential-barriers.png)

**[Figure 1](#image-activation-energy-potential-barriers). Synthetic potential-energy profiles: starting levels determine directional reaction energy barriers**. Original chosen profiles have [reactant](reactant.md) level $0$, [reaction product](product-chemistry.md) level $-20\,\mathrm{kJ\,mol^{-1}}$, and peak levels $80$ and $50\,\mathrm{kJ\,mol^{-1}}$. Forward [reaction energy barriers](reaction-energy-barrier.md) are $80$ and $50$; reverse [reaction energy barriers](reaction-energy-barrier.md) are $100$ and $70\,\mathrm{kJ\,mol^{-1}}$. The [reaction coordinate](reaction-coordinate.md) is not time. These curves are illustrative functions, not laboratory measurements or calculated molecular [potential energy surfaces](potential-energy-surface.md); their heights do not by themselves specify [Arrhenius activation energies](activation-energy.md).

A microscopic [reaction energy barrier](reaction-energy-barrier.md) belongs to a specified path on a [potential energy surface](potential-energy-surface.md). An experimental [activation energy](activation-energy.md) belongs to a specified [rate constant](rate-constant.md) and its [temperature](temperature-split.md) dependence. A multi-step [reaction mechanism](reaction-mechanism.md) can change which step controls the observed conversion, and a temperature-dependent [pre-exponential factor](pre-exponential-factor.md) contributes to the observed [activation energy](activation-energy.md). Even the [Gibbs energy of activation](gibbs-energy-of-activation.md) of [transition state theory](transition-state-theory.md) is a different quantity: it incorporates [entropy](entropy-split.md) as well as [enthalpy](enthalpy-split.md) and depends on the [standard states](standard-state.md). These distinctions prevent a fitted [Arrhenius plot](arrhenius-plot.md) from being mistaken for a direct microscopic energy measurement.[activation energy](iupac-compendium-of-chemical-terminology-fifth-edition-gold-book-by-international-union-of-pure-and-applied-chemistry/activation-energy.md)

[Catalysis](catalysis.md) illustrates the separation between a path and its endpoints. At the same [temperature](temperature-split.md) and with the same [reactants](reactant.md), [reaction products](product-chemistry.md), and [standard states](standard-state.md), a regenerated [catalyst](catalyst.md) changes the available [reaction mechanism](reaction-mechanism.md) and [rate constants](rate-constant.md), while the overall standard change in [Gibbs free energy](gibbs-free-energy.md) and the [equilibrium constant](equilibrium-constant.md) remain the same:

$$
K=\exp\left(-\frac{\Delta_rG^\circ}{RT}\right).
$$

For a reversible [first-order reaction](first-order-reaction.md) pair $\mathrm A\rightleftharpoons\mathrm B$, consistency at [chemical equilibrium](chemical-equilibrium.md) requires $k_f/k_r=K$. A model that multiplies only $k_f$ by a catalytic speedup while holding $k_r$ fixed would change this ratio and misrepresent [catalysis](catalysis.md). This simple ratio applies to that specified [rate law](rate-law.md); a multi-step catalytic [reaction mechanism](reaction-mechanism.md) needs its own rate equations. A [potential-energy profile](potential-energy-profile.md) alone cannot determine $K$, because its endpoint difference is not generally the standard change in [Gibbs free energy](gibbs-free-energy.md).[§13.3, Effect of a Catalyst: faster equilibration without changing equilibrium composition](chemistry-2e-by-paul-flowers-and-others/13-3-shifting-equilibria-le-chatelier%E2%80%99s-principle.md)

**Table of contents**

- [Apparent activation energy](apparent-activation-energy.md)
- [Arrhenius equation](arrhenius-equation.md)
  - [Two-temperature Arrhenius extrapolation](two-temperature-arrhenius-extrapolation.md)
  - [Pre-exponential factor](pre-exponential-factor.md)
  - [Arrhenius plot](arrhenius-plot.md)
  - [Modified Arrhenius equation](modified-arrhenius-equation.md)
  - [Conductometric determination of activation energy](conductometric-determination-of-activation-energy.md)

## ↑ Ancestors (4)

1. [Chemical kinetics](chemical-kinetics-split.md)
2. [Chemical reaction](chemical-reaction-split.md)
3. [Chemistry](chemistry-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (31)

- [Activation energy](activation-energy.md)
- [Apparent activation energy](apparent-activation-energy.md)
- [Arrhenius equation](arrhenius-equation.md)
- [Arrhenius plot](arrhenius-plot.md)
- [ATP-driven sugar phosphorylation](atp-driven-sugar-phosphorylation.md)
- [Bond-dissociation energy](bond-dissociation-energy.md)
- [Catalyst](catalyst.md)
- [Catalytic barriers and reaction free energy](catalytic-barriers-and-reaction-free-energy.md)
- [Coble creep](coble-creep.md)
- [Crystallographic defect](crystallographic-defect.md)
- [Energy coupling](energy-coupling.md)
- [Enthalpy cycle](enthalpy-cycle.md)
- [Hess's law](hess-s-law.md)
- [Homogeneous catalysis](homogeneous-catalysis.md)
- [Manganese dioxide peroxide contact demonstration](manganese-dioxide-peroxide-contact-demonstration.md)
- [Modified Arrhenius equation](modified-arrhenius-equation.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1/4/a/v/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-1/5/a/i/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-1/5/b/i/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/5/a/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-2a/section-b/23/g/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-3/section-d/42/d/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-3/section-d/42/e/solution.md)
- [Solution](past-exam-of-the-materials-science-course-of-the-university-of-cambridge/2016/paper-1/2/a/solution.md)
- [Solution](past-exam-of-the-materials-science-course-of-the-university-of-cambridge/2016/paper-1/7/a/solution.md)
- [Solution](past-exam-of-the-materials-science-course-of-the-university-of-cambridge/2022/paper-1/2/b/iii/solution.md)
- [Solution](past-exam-of-the-physics-of-the-earth-as-a-planet-course-of-the-university-of-cambridge/2015/paper-1/3/b/solution.md)
- [Solution](past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2018/section-b/b3/solution.md)
- [Pre-exponential factor](pre-exponential-factor.md)
- [Reaction energy barrier](reaction-energy-barrier.md)
- [Solvation thermodynamic balance](solvation-thermodynamic-balance.md)
