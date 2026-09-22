# Synthetic bimodal profile of a Bose gas

↑ **Parent:** [Dilute-gas Bose-Einstein condensation](dilute-gas-bose-einstein-condensation.md)

A broad component plus a narrow central component can have one local maximum while still displaying two distinct width scales. This is what “bimodal” means in this imaging context; it does not require two separated peaks. To isolate the population effect, construct an original normalized line profile

$$
G_\sigma(u)=\frac{e^{-u^2/(2\sigma^2)}}{\sqrt{2\pi}\sigma},\qquad
P(u)=(1-f_0)G_1(u)+f_0G_{0.20}(u).
$$

Both terms are [normal distributions](normal-distribution.md); their integrals are one, so the component areas are $1-f_0$ and $f_0$. With $f_0=0.488$, the narrow component has central height $f_0/(\sqrt{2\pi}\,0.20)\simeq0.9734$, while the broad component contributes $(1-f_0)/\sqrt{2\pi}\simeq0.2043$. A tall central feature therefore need not contain most of the particles. Holding these widths fixed deliberately isolates changing weights; it does not model how [temperature](temperature-split.md), interactions or camera resolution determine actual widths.

<a id="image-ideal-harmonic-trap-condensate-fraction-and-synthetic-profiles"></a>
![](bose-harmonic-trap-fraction-and-profiles.png)

**[Figure 6](#image-ideal-harmonic-trap-condensate-fraction-and-synthetic-profiles). Ideal harmonic-trap condensate fraction and synthetic profiles**. Original calculated [condensate fraction](condensate-fraction.md) at left; normalized two-width [normal distribution](normal-distribution.md) mixtures at right, with weights from the cubic law. Chosen widths and parameters, no measured data. A profile is a line marginal, not an unintegrated camera pixel cut.

For [absorption imaging](absorption-imaging.md) in the weak-probe regime with negligible saturation, the [optical depth](optical-depth.md) is $\mathrm{OD}(x,z)=-\ln[I(x,z)/I_0(x,z)]=\sigma_{\rm abs}n_{\rm col}(x,z)$, where $I_0$ is the reference [light intensity](light-intensity.md) without atoms, $I$ the transmitted [light intensity](light-intensity.md), $\sigma_{\rm abs}$ an effective absorption [cross section](cross-section-physics.md), and $n_{\rm col}$ the [column density](column-density.md). Integrating $n_{\rm col}$ over both image coordinates gives the particle number; a central pixel height alone does not. Finite resolution can obscure a narrow component, and saturation invalidates this simple logarithmic calibration.

## ↑ Ancestors (9)

1. [Dilute-gas Bose-Einstein condensation](dilute-gas-bose-einstein-condensation.md)
2. [Bose-Einstein condensation](bose-einstein-condensation.md)
3. [Bose-Einstein distribution](bose-einstein-distribution.md)
4. [Bose-Einstein statistics](bose-einstein-statistics.md)
5. [Quantum ideal-gas statistics](quantum-ideal-gas-statistics-split.md)
6. [Statistical physics](statistical-physics-split.md)
7. [Branches of physics](branches-of-physics.md)
8. [Physics](physics-split.md)
9. [Codex Wiki](split.md)
