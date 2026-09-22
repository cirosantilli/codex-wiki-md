# Apparent activation energy

↑ **Parent:** [Activation energy](activation-energy.md)

An [apparent activation energy](apparent-activation-energy.md) reports the [temperature](temperature.md) sensitivity of an observed [rate constant](rate-constant.md), without assuming that it equals one microscopic [reaction energy barrier](reaction-energy-barrier.md). The [chain rule](chain-rule.md) converts the empirical [activation energy](activation-energy.md) definition into the local slope of an [Arrhenius plot](arrhenius-plot.md):

$$
E_{a,\mathrm{app}}(T)=-R\frac{d\ln(k/k_{\mathrm{ref}})}{d(1/T)}.
$$

The fixed reference $k_{\mathrm{ref}}$ keeps the [natural logarithm](natural-logarithm.md) dimensionless. A fitted straight-line slope estimates this quantity over the chosen [temperature](temperature.md) interval; curvature means that one number does not describe every local slope.[activation energy](iupac-compendium-of-chemical-terminology-fifth-edition-gold-book-by-international-union-of-pure-and-applied-chemistry/activation-energy.md)

For the explicit model $k(T)=A(T)\exp[-E_0/(RT)]$ with constant exponent parameter $E_0$, differentiation gives

$$
E_{a,\mathrm{app}}(T)=E_0+RT^2\frac{d}{dT}\ln\frac{A(T)}{A(T_*)},
$$

where $T_*$ is fixed. The second term demonstrates why a microscopic interpretation needs more than a slope. If $E_0$ were itself allowed to depend on [temperature](temperature.md), differentiation would also contribute $-T\,dE_0/dT$; simply inserting a variable $E_0(T)$ and naming it the measured [activation energy](activation-energy.md) is generally incorrect.

An instructive [transition state theory](transition-state-theory.md) example for an effective [first-order reaction](first-order-reaction.md) is

$$
k(T)=\frac{k_{\mathrm B}T}{h}\exp\left(\frac{\Delta S^{\ddagger\circ}}{R}\right)\exp\left(-\frac{\Delta H^{\ddagger\circ}}{RT}\right).
$$

Here $k_{\mathrm B}$ and $h$ are the [Boltzmann constant](boltzmann-constant.md) and [Planck constant](planck-constant.md); $\Delta S^{\ddagger\circ}$ is the [entropy of activation](entropy-of-activation.md), and $\Delta H^{\ddagger\circ}$ the [enthalpy of activation](enthalpy-of-activation.md). With those two quantities constant over the chosen range and successful passage assumed, direct differentiation gives $E_{a,\mathrm{app}}=\Delta H^{\ddagger\circ}+RT$, while the [Gibbs energy of activation](gibbs-energy-of-activation.md) is $\Delta G^{\ddagger\circ}=\Delta H^{\ddagger\circ}-T\Delta S^{\ddagger\circ}$. These are three distinguishable quantities. The stated [first-order reaction](first-order-reaction.md) and fixed [standard states](standard-state.md) matter when comparing these formulas with measurements.[Glossary of Terms Used in Physical Organic Chemistry (IUPAC Recommendations 1994): E entries](glossary-of-terms-used-in-physical-organic-chemistry-iupac-recommendations-1994-e-entries.md)

## ↑ Ancestors (5)

1. [Activation energy](activation-energy.md)
2. [Chemical kinetics](chemical-kinetics.md)
3. [Chemical reaction](chemical-reaction.md)
4. [Chemistry](chemistry-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Apparent activation energy](apparent-activation-energy.md)
- [Arrhenius equation](arrhenius-equation.md)
- [Conductometric determination of activation energy](conductometric-determination-of-activation-energy.md)
- [Modified Arrhenius equation](modified-arrhenius-equation.md)
