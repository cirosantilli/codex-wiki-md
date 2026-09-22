# Conductometric determination of activation energy

↑ **Parent:** [Arrhenius equation](arrhenius-equation.md)

A concrete laboratory route to an [Arrhenius plot](arrhenius-plot.md) is to infer a [rate constant](rate-constant.md) at each controlled [temperature](temperature-split.md) from a changing [electrical conductivity](electrical-conductivity.md). The Technical University of Munich's [Activation Energy of a First-Order Reaction](laboratory-course-in-physical-chemistry-for-fundamental-studies-experiments-manual/activation-energy-of-a-first-order-reaction.md) supplies a teaching protocol, rather than a published set of measured [rate constants](rate-constant.md).

The manual follows [tertiary amylbromide](tert-amyl-bromide.md) conversion, which produces conducting [ions](ion.md). A measuring cell connects to a thermostat; an immersed [electrical conductivity](electrical-conductivity.md) probe also measures solution [temperature](temperature-split.md), and a magnetic stirrer mixes it. Use $80\,\mathrm{mL}$ of $80\%$ by volume [ethanol](ethanol.md) in [water](water.md), equilibrate, then add $0.5\,\mathrm{mL}$ of [tertiary amylbromide](tert-amyl-bromide.md). Record the baseline before addition and set time zero at addition. Repeat with fresh mixtures at $25$, $30$, and $35\,{}^\circ\mathrm C$, each within $\pm0.5\,{}^\circ\mathrm C$; record for $30$ minutes at the first two [temperatures](temperature-split.md) and until completion at the last. Clean the cell between runs and keep the added volume fixed. The completed $35\,{}^\circ\mathrm C$ mixture supplies endpoint [electrical conductivity](electrical-conductivity.md) measurements at the other [temperatures](temperature-split.md): one endpoint reading cannot be used unchanged at every [temperature](temperature-split.md).[pp. 82–84, §§8.2.5–8.3.2, and p. 85, §8.5.1: reaction, apparatus, temperatures, endpoint and baseline](laboratory-course-in-physical-chemistry-for-fundamental-studies-experiments-manual/activation-energy-of-a-first-order-reaction.md)

To see what is inferred from the readout, let $\sigma_0$, $\sigma(t)$, and $\sigma_\infty$ be the baseline, current, and completed-mixture [electrical conductivities](electrical-conductivity.md) at the same [temperature](temperature-split.md). Assume their baseline-subtracted changes are proportional to converted [concentration](concentration.md). Combining that measurement model with a [first-order reaction](first-order-reaction.md) gives

$$
f(t)=\frac{\sigma_\infty-\sigma(t)}{\sigma_\infty-\sigma_0}
=\frac{c(t)}{c_0}=e^{-kt},
\qquad -\ln f(t)=kt.
$$

Thus the [electrical conductivity](electrical-conductivity.md) increases toward an endpoint, while the remaining [reactant](reactant.md) fraction decreases. Fit $-\ln f$ against time to obtain $k$; then fit $\ln(k/k_{\mathrm{ref}})$ against $1/T$ in [kelvin](kelvin.md) to estimate an [apparent activation energy](apparent-activation-energy.md). This baseline-aware derivation states the measurement assumptions explicitly; it does not infer a [rate constant](rate-constant.md) from the steepness of a raw conductivity trace alone.

The controls distinguish a faster [chemical reaction](chemical-reaction-split.md) from a larger instrumental response. Measure the actual solution [temperature](temperature-split.md), retain the same [solvent](solvent.md) composition and initial [reactant](reactant.md) [concentration](concentration.md), and compare endpoint and baseline at that [temperature](temperature-split.md). As further diagnostic checks, repeat runs and inspect [regression residuals](regression-residual.md) for departure from a [first-order reaction](first-order-reaction.md). These checks follow from the model: [electrical conductivity](electrical-conductivity.md) also depends on how [ions](ion.md) move, a baseline drift can mimic conversion, and a mixing delay can distort early points. Near completion, a small endpoint error produces a large relative error in $f$ and its [natural logarithm](natural-logarithm.md). A successful fit supports an apparent rate model for this [solvent](solvent.md) and interval; it does not directly image a [transition state](transition-state.md) or identify a unique [reaction mechanism](reaction-mechanism.md). No measured $k$ or $E_a$ is supplied here.

## ↑ Ancestors (6)

1. [Arrhenius equation](arrhenius-equation.md)
2. [Activation energy](activation-energy.md)
3. [Chemical kinetics](chemical-kinetics-split.md)
4. [Chemical reaction](chemical-reaction-split.md)
5. [Chemistry](chemistry-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Tert-amyl bromide](tert-amyl-bromide.md)
