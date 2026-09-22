# Gibbs free energy

↑ **Parent:** [Thermodynamic free energy](thermodynamic-free-energy.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gibbs_free_energy)

The [Gibbs free energy](gibbs-free-energy.md) is

$$
G=U-TS+pV=H-TS,\qquad H=U+pV,
$$

where $H$ is [enthalpy](enthalpy.md). For a [closed system](closed-system.md) of fixed composition, with only [pressure](pressure.md)-[volume](volume-thermodynamics.md) [work](work.md), spontaneous relaxation at fixed [temperature](temperature.md) and [pressure](pressure.md) cannot increase $G$; stable [thermodynamic equilibrium](thermodynamic-equilibrium.md) minimizes it over the allowed states. A loaded piston can move while maintaining the imposed [pressure](pressure.md), so the [enthalpy](enthalpy.md) term includes the displacement cost. Along a smooth equilibrium branch of fixed composition,

$$
dG=-S\,dT+V\,dp.
$$

Thus its [temperature](temperature.md) slope at fixed [pressure](pressure.md) is $-S$, while its [pressure](pressure.md) slope at fixed [temperature](temperature.md) is $V$. See [MIT 5.60, Lecture 13, Gibbs free energy and its derivatives](https://ocw.mit.edu/courses/5-60-thermodynamics-kinetics-spring-2008/7bc33304ab1db561a64b4a6b12e25476_5_60_lecture13.pdf).

Consider two illustrative [thermodynamic phases](thermodynamic-phase.md), A and B, of the same substance at one fixed [pressure](pressure.md). Write B minus A, using quantities per [mole](mole-unit.md):

$$
\Delta H=12\,\mathrm{kJ\,mol^{-1}},\qquad
\Delta S=40\,\mathrm{J\,mol^{-1}\,K^{-1}}=0.040\,\mathrm{kJ\,mol^{-1}\,K^{-1}}.
$$

Treat these differences as approximately constant over a limited [temperature](temperature.md) window. Then

$$
\frac{\Delta G(T)}{\mathrm{kJ\,mol^{-1}}}=12-0.040\frac{T}{\mathrm K},\qquad
T_* =\frac{\Delta H}{\Delta S}=300\,\mathrm K.
$$

At $280\,\mathrm K$, $\Delta G=+0.8\,\mathrm{kJ\,mol^{-1}}$, so A is preferred. At $320\,\mathrm K$, $\Delta G=-0.8\,\mathrm{kJ\,mol^{-1}}$, so B is preferred. At $300\,\mathrm K$, both have equal molar [Gibbs free energy](gibbs-free-energy.md), permitting [phase coexistence](phase-coexistence.md) in this bulk model. B's greater [entropy](entropy.md) outweighs its greater [enthalpy](enthalpy.md) above the crossing.

<a id="image-illustrative-molar-gibbs-free-energy-difference-crosses-zero-at-300-mathrm-k"></a>
![](free-energy-temperature-crossing.png)

**[Figure 45](#image-illustrative-molar-gibbs-free-energy-difference-crosses-zero-at-300-mathrm-k). Illustrative molar Gibbs free energy difference crosses zero at $300\,\mathrm K$**. Constructed B-minus-A values: $+0.8\,\mathrm{kJ\,mol^{-1}}$ at $280\,\mathrm K$ and $-0.8\,\mathrm{kJ\,mol^{-1}}$ at $320\,\mathrm K$. The constants approximate a limited [temperature](temperature.md) window and represent no measured substance.

Each plotted point compares alternatives at the same [temperature](temperature.md); moving along the curve changes the imposed [temperature](temperature.md). The model predicts preference, not instantaneous conversion: [nucleation](nucleation.md) barriers can sustain [metastability](metastability.md). Real [enthalpy](enthalpy.md) and [entropy](entropy.md) differences generally vary with [temperature](temperature.md) through [heat capacities](heat-capacity.md), bending this line outside the approximation.

At fixed [pressure](pressure.md), the [first law of thermodynamics](first-law-of-thermodynamics.md) gives $Q=\Delta H$ under the stated [work](work.md) restriction, so the same [thermal reservoir](heat-bath.md) accounting yields $\Delta S_{\rm total}=-\Delta G/T\geq0$. Variable composition restores $\sum_i\mu_i\,dn_i$ to $dG$; [constrained Gibbs minimization for chemical equilibrium](constrained-gibbs-minimization-for-chemical-equilibrium.md) handles those permitted changes.

The historical foundation is Gibbs's [On the Equilibrium of Heterogeneous Substances, first part completed in 1876, continued in 1878](https://en.wikisource.org/wiki/Scientific_Papers_of_Josiah_Willard_Gibbs,_Volume_1/Chapter_IIIa). Its equations (87) and (91) introduce the combinations now called [Helmholtz free energy](helmholtz-free-energy.md) and [Gibbs free energy](gibbs-free-energy.md), connecting [entropy](entropy.md) criteria, [chemical potentials](chemical-potential.md) and [phase coexistence](phase-coexistence.md) within one framework.

**Table of contents**

- [Gibbs free energy of an ideal-gas mixture](gibbs-free-energy-of-an-ideal-gas-mixture.md)
- [Gibbs free-energy Maxwell relation](gibbs-free-energy-maxwell-relation.md)
- [Chemical-potential balance for a reaction](chemical-potential-balance-for-a-reaction.md)
  - [Thermochemical equilibrium](thermochemical-equilibrium.md)
    - [Constrained Gibbs minimization for chemical equilibrium](constrained-gibbs-minimization-for-chemical-equilibrium.md)
    - [Reverse reaction rate from equilibrium thermodynamics](reverse-reaction-rate-from-equilibrium-thermodynamics.md)
- [Phase coexistence curve](phase-coexistence-curve.md)
  - [Triple point](triple-point.md)
  - [Vapor pressure](vapor-pressure.md)
  - [Maxwell construction](maxwell-construction.md)
  - [Phase diagram](phase-diagram.md)
    - [Solidus](solidus.md)
    - [Lever rule](lever-rule.md)
    - [Bicritical point](bicritical-point.md)
    - [Liquidus](liquidus.md)
      - [Freezing-point depression](freezing-point-depression.md)
    - [Eutectic system](eutectic-system.md)
      - [Eutectic composition](eutectic-composition.md)
      - [Eutectic temperature](eutectic-temperature.md)
  - [First-order phase transition](first-order-phase-transition.md)
    - [Two-phase scalar coexistence endpoint conditions](two-phase-scalar-coexistence-endpoint-conditions.md)
    - [Spin-flop transition](spin-flop-transition.md)
    - [Classical nucleation theory](classical-nucleation-theory.md)
      - [Critical nucleus](critical-nucleus.md)
      - [Arrhenius nucleation time](arrhenius-nucleation-time.md)
  - [Latent heat](latent-heat.md)
    - [Stefan number](stefan-number.md)
      - [Latent-to-sensible heat ratio](latent-to-sensible-heat-ratio.md)
    - [Clausius-Clapeyron relation](clausius-clapeyron-relation.md)
      - [Ideal-vapor Clausius-Clapeyron approximation](ideal-vapor-clausius-clapeyron-approximation.md)
        - [Integrated Clausius-Clapeyron relation](integrated-clausius-clapeyron-relation.md)
          - [Stipulated vapor-pressure calculation](stipulated-vapor-pressure-calculation.md)
          - [Latent heat from a vapor-pressure slope](latent-heat-from-a-vapor-pressure-slope.md)
      - [Saturation-pressure equilibrium measurement](saturation-pressure-equilibrium-measurement.md)
      - [Common-pressure melting-point slope](common-pressure-melting-point-slope.md)
        - [Negative melting-point slope of water](negative-melting-point-slope-of-water.md)

## ↑ Ancestors (7)

1. [Thermodynamic free energy](thermodynamic-free-energy.md)
2. [Thermodynamic potential](thermodynamic-potential.md)
3. [Thermodynamics](thermodynamics-split.md)
4. [Statistical physics](statistical-physics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (56)

- [Activation energy](activation-energy.md)
- [Adenosine triphosphate](adenosine-triphosphate.md)
- [Base pairing](base-pairing.md)
- [Catalysis](catalysis.md)
- [Catalyst](catalyst.md)
- [Catalytic barriers and reaction free energy](catalytic-barriers-and-reaction-free-energy.md)
- [Chemical equilibrium](chemical-equilibrium.md)
- [Chemical kinetics](chemical-kinetics.md)
- [Chemical potential](chemical-potential.md)
- [Chemical potential and Helmholtz free energy](chemical-potential-and-helmholtz-free-energy.md)
- [Chemical potential equality for particle exchange](chemical-potential-equality-for-particle-exchange.md)
- [Clausius-Clapeyron relation](clausius-clapeyron-relation.md)
- [Constrained Gibbs minimization for chemical equilibrium](constrained-gibbs-minimization-for-chemical-equilibrium.md)
- [Daniell cell](daniell-cell.md)
- [Desolvation](desolvation.md)
- [Electrolysis](electrolysis.md)
- [Electrolytic cell](electrolytic-cell.md)
- [Endergonic reaction](endergonic-reaction.md)
- [Energy coupling](energy-coupling.md)
- [Energy profile (chemistry)](energy-profile-chemistry.md)
- [Enzyme](enzyme.md)
- [Equilibrium constant](equilibrium-constant.md)
- [Exergonic reaction](exergonic-reaction.md)
- [Gibbs energy of activation](gibbs-energy-of-activation.md)
- [Gibbs free energy](gibbs-free-energy.md)
- [Gibbs free energy of an ideal-gas mixture](gibbs-free-energy-of-an-ideal-gas-mixture.md)
- [Hydrogen bond acceptor](hydrogen-bond-acceptor.md)
- [Hydrophobic effect](hydrophobic-effect.md)
- [Isothermal compressibility](isothermal-compressibility.md)
- [Latent heat](latent-heat.md)
- [Latent heat of fusion](latent-heat-of-fusion.md)
- [Maxwell relations](maxwell-relations.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-4/34d/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-3/33c/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-303/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-315/2/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-315/2/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-315/4/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-315/4/f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-315/4/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-4/35a/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-315/2/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-2/37a/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-315/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-4/35b/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ii/paper-4/35c/a/solution.md)
- [Physical properties of salts](physical-properties-of-salts.md)
- [Protein folding](protein-folding.md)
- [Reversible catalytic relaxation](reversible-catalytic-relaxation.md)
- [Solubility](solubility.md)
- [Solvation free energy](solvation-free-energy.md)
- [Solvation thermodynamic balance](solvation-thermodynamic-balance.md)
- [Thermodynamic equilibrium](thermodynamic-equilibrium.md)
- [Thermodynamic free energy](thermodynamic-free-energy.md)
- [Thermodynamic potential](thermodynamic-potential.md)
- [Transition state](transition-state.md)
