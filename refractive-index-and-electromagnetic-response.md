# Refractive index and electromagnetic response

↑ **Parent:** [Refractive index](refractive-index.md)

For a uniform linear medium with [isotropy](isotropy.md) and local constitutive response, [Maxwell equations](maxwell-equations-split.md) give $k^2=\omega^2\varepsilon(\omega)\mu(\omega)$. Here $\varepsilon$ is [permittivity](permittivity-split.md) and $\mu$ is [magnetic permeability](permeability-electromagnetism.md). Since $c^{-2}=\varepsilon_0\mu_0$, the [relative permittivity](relative-permittivity.md) $\varepsilon_r=\varepsilon/\varepsilon_0$ and the relative [magnetic permeability](permeability-electromagnetism.md) $\mu_r=\mu/\mu_0$ obey

$$
n^2=\varepsilon_r\mu_r.
$$

If both responses are real and positive with negligible loss, and the ordinary positive-index branch is intended, then $n=+\sqrt{\varepsilon_r\mu_r}$. If additionally $\mu_r\simeq1$, then $n\simeq\sqrt{\varepsilon_r}$. All these responses must be evaluated at the [electromagnetic wave](electromagnetic-wave-split.md)'s [frequency](frequency.md); a static [relative permittivity](relative-permittivity.md) cannot simply be substituted at an optical [frequency](frequency.md). [RP Photonics Encyclopedia by Rüdiger Paschotta; What is a Refractive Index?: squared constitutive relation and frequency-specific material responses](rp-photonics-encyclopedia-by-rudiger-paschotta/refractive-index.md)

With loss, use a complex index $\widetilde n=n'+i\kappa$ and explicitly fix the [phase convention for complex amplitudes](phase-convention-for-complex-amplitudes.md). For $E\propto\exp[i(kz-\omega t)]$ with $k=\widetilde n\omega/c$, its [wave amplitude](wave-amplitude.md) has factor $\exp(-\kappa\omega z/c)$. A forward attenuating branch has $\kappa\geq0$, while its [wave phase](phase-waves.md) is controlled by $n'$. The complex relation $\widetilde n^2=\varepsilon_r\mu_r$ alone leaves a choice of sign: the physical solution also needs [causality](causality.md) and the appropriate radiation or decay condition. In negative-index media the physically selected real part can be negative. The positive square root is therefore not a universal rule for complex or negative-index media. Direction and [polarization of an electromagnetic wave](polarization-of-an-electromagnetic-wave.md) also matter in a [plane wave in an anisotropic dielectric](plane-wave-in-an-anisotropic-dielectric.md), for which one scalar index need not describe every propagation branch.

## ↑ Ancestors (6)

1. [Refractive index](refractive-index.md)
2. [Electromagnetic wave](electromagnetic-wave-split.md)
3. [Electromagnetism](electromagnetism-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Refractive index](refractive-index.md)
