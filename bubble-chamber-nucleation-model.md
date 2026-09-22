# Bubble-chamber nucleation model

↑ **Parent:** [Bubble chamber](bubble-chamber.md)

Why can hot [liquid](liquid.md) wait for a [charged particle](charged-particle.md) rather than immediately turn into [vapor](vapor.md)? A small cavity costs [surface energy](surface-energy.md). Consider an original macroscopic capillarity model at fixed [temperature](temperature-split.md) with [surface tension](surface-tension-split.md) $\sigma>0$, imposed [liquid](liquid.md) [pressure](pressure-split.md) $p_l$, and driving difference $\Delta p=p_{\rm sat}(T)-p_l>0$, where $p_{\rm sat}$ is the planar-interface [vapor pressure](vapor-pressure.md). Neglect dissolved [gas](gas.md), interface thickness, [heat transfer](heat-transfer.md) and curvature dependence of $\sigma$. The reversible formation-work approximation is

$$
\Delta G(r)=4\pi\sigma r^2-\frac{4\pi}{3}\Delta p\,r^3.
$$

The first term charges for surface area; the second rewards the new [vapor](vapor.md) [volume](volume-thermodynamics.md). This is a macroscopic [free energy](thermodynamic-free-energy.md) model, not the [energy](energy-split.md) that an actual detector must receive as localized [heat](heat-split.md). It shares the capillarity balance used in the [cloud-chamber expansion model](cloud-chamber-expansion-model.md), but the new phase is now a bubble.

Differentiating gives

$$
\frac{d\Delta G}{dr}=4\pi r(2\sigma-\Delta p\,r),\qquad
r_* =\frac{2\sigma}{\Delta p},\qquad
\Delta G_* =\frac{16\pi\sigma^3}{3\Delta p^2}.
$$

At the [critical nucleus](critical-nucleus.md), $d^2\Delta G/dr^2=-8\pi\sigma<0$. The barrier is a maximum: cavities smaller than $r_*$ tend to shrink, while larger ones can grow in this model. Doubling $\Delta p$ halves $r_*$ and quarters $\Delta G_*$ if $\sigma$ stays fixed. This explains the strong sensitivity to operating conditions without claiming a universal detector threshold.

Choose $\sigma=0.010\,\mathrm{J\,m^{-2}}$ and $\Delta p=2.0\times10^5\,\mathrm{Pa}$ solely for a teaching example. Then

$$
r_*=100\,\mathrm{nm},\qquad
\Delta G_*=4.189\times10^{-16}\,\mathrm J\simeq2.614\,\mathrm{keV}.
$$

For the same chosen $\sigma$ and twice the driving [pressure](pressure-split.md), $r_*=50\,\mathrm{nm}$ and $\Delta G_*\simeq0.654\,\mathrm{keV}$. These are calculated formation-work scales, not measured bubble thresholds for [diethyl ether](diethyl-ether.md) or any other substance.

<a id="image-surface-energy-and-bulk-driving-compete-to-set-a-bubble-s-critical-nucleus"></a>
![](bubble-chamber-critical-radius-model.png)

**[Figure 14](#image-surface-energy-and-bulk-driving-compete-to-set-a-bubble-s-critical-nucleus). Surface energy and bulk driving compete to set a bubble's critical nucleus**. Original calculations for stipulated surface tension and pressure differences. The plotted formation work is neither measured data nor a complete radiation-response model.

A simplified way to discuss localization is to stipulate deposited [energy](energy-split.md) $E_{\rm loc}$ within a segment of [length](length.md) $\ell$ and a trial conversion fraction $0<\eta\leq1$. A toy criterion $\eta E_{\rm loc}\gtrsim\Delta G_*$ gives an [energy](energy-split.md) per unit [length](length.md) scale $\Delta G_*/(\eta\ell)$. It is only a bookkeeping estimate: a real bubble also needs [latent heat](latent-heat.md), must exchange [heat](heat-split.md), and is affected by the spatial pattern and time scale of [energy](energy-split.md) deposition. Consequently neither a single [stopping power](stopping-power.md) value nor this barrier alone predicts [detection efficiency](detection-efficiency.md) or the number of bubbles. Two tracks with the same mean [stopping power](stopping-power.md) can distribute their [energy](energy-split.md) differently on the scale of a [critical nucleus](critical-nucleus.md).

## ↑ Ancestors (5)

1. [Bubble chamber](bubble-chamber.md)
2. [Particle detector](particle-detector.md)
3. [Particle detection](particle-detection-split.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)
