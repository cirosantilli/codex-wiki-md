# Beam hardening

↑ **Parent:** [X-ray attenuation](x-ray-attenuation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Beam_hardening)

An original two-[energy](energy-split.md) model demonstrates the failure of a single constant [linear attenuation coefficient](linear-attenuation-coefficient.md) for a mixed beam. Suppose the two components contribute equally to the empty-path detector signal and have stipulated $\mu_1=0.40\,\mathrm{mm^{-1}}$ and $\mu_2=0.10\,\mathrm{mm^{-1}}$. With fixed linear detector response and no accepted [scattering of light](scattering-of-light.md),

$$
T(x)=\frac12e^{-\mu_1x}+\frac12e^{-\mu_2x},\qquad
-\frac{d\ln T}{dx}
=\frac{\mu_1e^{-\mu_1x}+\mu_2e^{-\mu_2x}}
{e^{-\mu_1x}+e^{-\mu_2x}}.
$$

The initial slope corresponds to $\mu=0.25\,\mathrm{mm^{-1}}$, but at $x=5\,\mathrm{mm}$, $T\simeq0.371$, rather than $e^{-0.25(5)}\simeq0.287$. The more strongly attenuated component disappears faster. If that component has lower [photon](photon.md) [energy](energy-split.md), the surviving beam has a higher mean [energy](energy-split.md): [beam hardening](beam-hardening.md). The formula is explicitly a two-component example, not a universal rule that attenuation decreases monotonically with [photon](photon.md) [energy](energy-split.md). Detector weighting also matters when interpreting a broadband transmission signal.

## ↑ Ancestors (7)

1. [X-ray attenuation](x-ray-attenuation.md)
2. [X-ray](x-ray.md)
3. [Electromagnetic radiation](electromagnetic-radiation-split.md)
4. [Electromagnetism](electromagnetism-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Beam hardening](beam-hardening.md)
