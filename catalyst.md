# Catalyst

↑ **Parent:** [Catalysis](catalysis.md)

A [catalyst](catalyst.md) makes a [chemical reaction](chemical-reaction-split.md) proceed faster by participating in an alternative [reaction mechanism](reaction-mechanism.md) and being regenerated. This makes repeated conversion possible: the same [catalyst](catalyst.md) can help many successive [reactants](reactant.md) become [reaction products](product-chemistry.md). An [enzyme](enzyme-split.md) is a biological [catalyst](catalyst.md). The overall standard change in [Gibbs free energy](gibbs-free-energy.md) is unchanged; see the [IUPAC Gold Book: catalyst](https://goldbook.iupac.org/terms/view/C00876).

Regeneration does not mean that the [catalyst](catalyst.md) sits unchanged throughout every step. For example, a schematic [reaction mechanism](reaction-mechanism.md) can temporarily bind A to a [catalyst](catalyst.md) C in a [reaction intermediate](reaction-intermediate.md) AC:

$$
\begin{aligned}
\mathrm A+\mathrm C&\rightleftharpoons\mathrm{AC},\\
\mathrm{AC}&\rightleftharpoons\mathrm B+\mathrm C,\\
\text{net:}\qquad\mathrm A&\rightleftharpoons\mathrm B.
\end{aligned}
$$

Adding the steps cancels both the [reaction intermediate](reaction-intermediate.md) AC and the [catalyst](catalyst.md) C from the net [chemical equation](chemical-equation.md). AC is produced and later consumed; C is used and later recovered. These letters describe possible roles, not a measured [reaction mechanism](reaction-mechanism.md). The alternative route is useful only if its [chemical kinetics](chemical-kinetics-split.md) permits faster conversion. See [Flowers et al., Chemistry 2e, §12.7: catalysts and alternative mechanisms](https://openstax.org/books/chemistry-2e/pages/12-7-catalysis).

For a worked barrier example, consider an idealized reversible A-to-B conversion at fixed [temperature](temperature-split.md) $T=300\,\mathrm K$. Stipulate standard molar [Gibbs free energy](gibbs-free-energy.md) levels $G_{\mathrm A}^\circ=0$ and $G_{\mathrm B}^\circ=-20\,\mathrm{kJ\,mol^{-1}}$, with effective [transition state](transition-state.md) levels $80$ without a [catalyst](catalyst.md) and $50\,\mathrm{kJ\,mol^{-1}}$ with a [catalyst](catalyst.md). Use the same [standard states](standard-state.md) and the same zero for both routes; the catalytic route includes the regenerated C at both endpoints. Unlike the separate [potential-energy profile](potential-energy-profile.md) example, this illustration uses [Gibbs free energy](gibbs-free-energy.md) at one specified [temperature](temperature-split.md).

<a id="image-a-catalyst-lowers-the-stipulated-gibbs-energy-of-activation-in-both-directions-while-retaining-the-same-endpoints"></a>
![](catalyst-alternative-reaction-path.png)

**[Figure 11](#image-a-catalyst-lowers-the-stipulated-gibbs-energy-of-activation-in-both-directions-while-retaining-the-same-endpoints). A catalyst lowers the stipulated Gibbs energy of activation in both directions while retaining the same endpoints**. Original smooth schematic [Gibbs free energy](gibbs-free-energy.md) profiles at $300\,\mathrm K$, with levels in $\mathrm{kJ\,mol^{-1}}$. The horizontal [reaction coordinate](reaction-coordinate.md) describes progress along each schematic route, not time. These are chosen effective barriers, not measured [potential energy surfaces](potential-energy-surface.md), actual molecular paths, or the two-step [reaction mechanism](reaction-mechanism.md) above. A real catalytic route can have several [transition states](transition-state.md) and [reaction intermediates](reaction-intermediate.md).

The [Gibbs energy of activation](gibbs-energy-of-activation.md) is measured from the starting endpoint in the chosen direction. Thus the four barriers are

$$
\begin{aligned}
\Delta G_{f,\mathrm{uncat}}^{\ddagger\circ}&=80-0=80,&
\Delta G_{f,\mathrm{cat}}^{\ddagger\circ}&=50-0=50,\\
\Delta G_{r,\mathrm{uncat}}^{\ddagger\circ}&=80-(-20)=100,&
\Delta G_{r,\mathrm{cat}}^{\ddagger\circ}&=50-(-20)=70,
\end{aligned}
\qquad\text{all in }\mathrm{kJ\,mol^{-1}}.
$$

Both directional barriers fall by $30\,\mathrm{kJ\,mol^{-1}}$. The endpoint difference stays $\Delta_rG^\circ=-20\,\mathrm{kJ\,mol^{-1}}$.

To turn those barriers into [rate constants](rate-constant.md), use the Eyring form of [transition state theory](transition-state-theory.md) for this effective [first-order reaction](first-order-reaction.md) pair, with a common prefactor and unit probability of successful passage:

$$
k=\nu\exp\left(-\frac{\Delta G^{\ddagger\circ}}{RT}\right),
\qquad \nu=\frac{k_{\mathrm B}T}{h}.
$$

Here $k_{\mathrm B}$ is the [Boltzmann constant](boltzmann-constant.md), $h$ is the [Planck constant](planck-constant.md), and $R$ is the [molar gas constant](molar-gas-constant.md). The common prefactor cancels from the comparisons. These [Gibbs energies of activation](gibbs-energy-of-activation.md) are not the empirical [activation energy](activation-energy.md) $E_a$ of the [Arrhenius equation](arrhenius-equation.md). With the stipulated value $R=8.314462618\,\mathrm{J\,mol^{-1}\,K^{-1}}$, the speedup is

$$
\frac{k_{f,\mathrm{cat}}}{k_{f,\mathrm{uncat}}}
=\frac{k_{r,\mathrm{cat}}}{k_{r,\mathrm{uncat}}}
=\exp\left(\frac{30000}{8.314462618\times300}\right)
\approx1.67248\times10^5.
$$

The exponent is a [dimensionless quantity](dimensionless-quantity.md): convert $30\,\mathrm{kJ\,mol^{-1}}$ to $30000\,\mathrm{J\,mol^{-1}}$ before dividing by $RT$. The [exponential function](exponential-function.md) explains why a modest barrier reduction can have a dramatic kinetic effect. This number follows from the chosen free-energy barriers and common prefactor; it is not a universal catalytic multiplier or a prediction across [temperatures](temperature-split.md).

<a id="image-both-directional-rate-constants-increase-by-about-1-67-times10-5-while-their-forward-to-reverse-ratio-stays-about-3036"></a>
![](catalyst-forward-reverse-rate-ratios.png)

**[Figure 12](#image-both-directional-rate-constants-increase-by-about-1-67-times10-5-while-their-forward-to-reverse-ratio-stays-about-3036). Both directional rate constants increase by about $1.67\times10^5$, while their forward-to-reverse ratio stays about $3036$**. Original bar plots at $300\,\mathrm K$. Left: base-ten [logarithms](logarithm.md) of the [dimensionless](dimensionless-quantity.md) normalized [rate constants](rate-constant.md) $k/\nu$ for the four stipulated barriers. A less negative value means faster conversion. Right: the [logarithm](logarithm.md) of $k_f/k_r$ is identical for the two routes. Absolute units factor out through the common $\nu=k_{\mathrm B}T/h$; no temperature dependence outside this one model point is asserted.

Assume ideal [thermodynamic activities](thermodynamic-activity.md) with a common concentration [standard state](standard-state.md), and directional [rate laws](rate-law.md) $J_f=k_f[\mathrm A]$ and $J_r=k_r[\mathrm B]$. At [chemical equilibrium](chemical-equilibrium.md), equal [reaction rates](reaction-rate.md) give $K=[\mathrm B]/[\mathrm A]=k_f/k_r$ for this model. The barriers give

$$
K_{\mathrm{uncat}}=\frac{e^{-80000/(RT)}}{e^{-100000/(RT)}}
=e^{20000/(RT)}
=\frac{e^{-50000/(RT)}}{e^{-70000/(RT)}}=K_{\mathrm{cat}}
\approx3035.58.
$$

The [catalyst](catalyst.md) speeds up both directions, so it changes how quickly [chemical equilibrium](chemical-equilibrium.md) is approached without changing this [equilibrium constant](equilibrium-constant.md). For a general [chemical reaction](chemical-reaction-split.md), the thermodynamic relation is $K=\exp[-\Delta_rG^\circ/(RT)]$ with consistent [standard states](standard-state.md); an arbitrary multistep [reaction mechanism](reaction-mechanism.md) need not permit $K=k_f/k_r$ for two measured [rate constants](rate-constant.md). At the same [temperature](temperature-split.md), [pressure](pressure-split.md), and [thermodynamic activities](thermodynamic-activity.md), a [catalyst](catalyst.md) also leaves the actual overall reaction change in [Gibbs free energy](gibbs-free-energy.md) unchanged. See [13.3 Shifting Equilibria: Le Châtelier’s Principle](chemistry-2e-by-paul-flowers-and-others/13-3-shifting-equilibria-le-chatelier%E2%80%99s-principle.md) (§13.3: a catalyst does not shift equilibrium). To drive an unfavourable overall conversion, a process such as [energy coupling](energy-coupling.md) must change the combined transformation.

**Table of contents**

- [Precatalyst](precatalyst.md)
- [Transition state theory](transition-state-theory.md)
  - [Force-tilted activation barrier](force-tilted-activation-barrier.md)
  - [Activation volume](activation-volume.md)
  - [Activation entropy](activation-entropy.md)
  - [Activation enthalpy](activation-enthalpy.md)
  - [Eyring equation](eyring-equation.md)
  - [Gibbs energy of activation](gibbs-energy-of-activation.md)
    - [Enthalpy of activation](enthalpy-of-activation.md)
    - [Entropy of activation](entropy-of-activation.md)

## ↑ Ancestors (5)

1. [Catalysis](catalysis.md)
2. [Chemical kinetics](chemical-kinetics-split.md)
3. [Chemical reaction](chemical-reaction-split.md)
4. [Chemistry](chemistry-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (42)

- [Activation energy](activation-energy.md)
- [Adenosine diphosphate](adenosine-diphosphate.md)
- [Catalysed peroxide comparison](catalysed-peroxide-comparison.md)
- [Catalysis](catalysis.md)
- [Catalyst](catalyst.md)
- [Catalyst deactivation](catalyst-deactivation.md)
- [Catalyst particle size and accessible area](catalyst-particle-size-and-accessible-area.md)
- [Catalyst-transfer polymerization](catalyst-transfer-polymerization.md)
- [Catalytic barriers and reaction free energy](catalytic-barriers-and-reaction-free-energy.md)
- [Catalytic cycle](catalytic-cycle.md)
- [Catalytic selectivity](catalytic-selectivity.md)
- [Chemical kinetics](chemical-kinetics-split.md)
- [Copper(II) sulfate](copper-ii-sulfate.md)
- [Enzyme](enzyme-split.md)
- [Guanosine](guanosine.md)
- [Heat released by hydrogen spin conversion](heat-released-by-hydrogen-spin-conversion.md)
- [Hess's law](hess-s-law.md)
- [Heterogeneous catalysis](heterogeneous-catalysis.md)
- [Homogeneous catalysis](homogeneous-catalysis.md)
- [Methylaluminoxane](methylaluminoxane.md)
- [Normal hydrogen](normal-hydrogen.md)
- [Solution](past-exam-of-the-chemistry-b-course-of-the-university-of-cambridge/2022/paper-1/b1/a/iii/solution.md)
- [Solution](past-exam-of-the-chemistry-b-course-of-the-university-of-cambridge/2022/paper-1/b3/b/solution.md)
- [Solution](past-exam-of-the-chemistry-b-course-of-the-university-of-cambridge/2022/paper-2/b8/c/i/solution.md)
- [Solution](past-exam-of-the-chemistry-b-course-of-the-university-of-cambridge/2022/paper-2/b8/c/iii/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/3/c/i/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1/10/a/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1/10/b/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1/14/a/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1/14/b/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1/14/d/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1/16/b/solution.md)
- [Solution](past-exam-of-the-mphil-in-micro-and-nanotechnology-enterprise-course-of-the-university-of-cambridge/2017/paper-2/section-b/20/i/solution.md)
- [Solution](past-exam-of-the-mphil-in-micro-and-nanotechnology-enterprise-course-of-the-university-of-cambridge/2019/paper-2/section-a-i/14/i/solution.md)
- [Solution](past-exam-of-the-mphil-in-micro-and-nanotechnology-enterprise-course-of-the-university-of-cambridge/2019/paper-2/section-b/20/iii/solution.md)
- [PCR thermal cycle](pcr-thermal-cycle.md)
- [Reaction intermediate](reaction-intermediate.md)
- [Reaction mechanism](reaction-mechanism.md)
- [Ribozyme](ribozyme.md)
- [Saponification](saponification.md)
- [Surface-catalysed hydrogen spin conversion experiment](surface-catalysed-hydrogen-spin-conversion-experiment.md)
- [Transition state theory](transition-state-theory.md)
