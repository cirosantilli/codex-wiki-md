# Finite-band Cherenkov yield model

↑ **Parent:** [Frank-Tamm formula](frank-tamm-formula.md)

Choose an original transparent-band model, defined only for $400\leq\lambda\leq700\,\mathrm{nm}$:

$$
n(\lambda)=1.28+0.04\left(\frac{500\,\mathrm{nm}}\lambda\right)^2.
$$

This chosen [refractive index](refractive-index.md) is not a fit to water, glass or the historical liquids. It decreases from $1.3425$ to approximately $1.300408$, so the threshold $1/n$ increases across the band. For $\beta=0.75$, solving $n(\lambda_*)=1/\beta$ gives

$$
\lambda_*=500\sqrt{\frac{0.04}{1/0.75-1.28}}\,\mathrm{nm}
\simeq433.013\,\mathrm{nm}.
$$

Only $400\leq\lambda<\lambda_*$ emits. Faster particles with $\beta=0.78$ and $0.90$ emit throughout this chosen band. The [Cherenkov cone angle](cherenkov-cone-angle.md) and the [Frank-Tamm formula](frank-tamm-formula.md) are both evaluated with the same $n(\lambda)$.

<a id="image-original-dispersive-cherenkov-radiation-model-a-wavelength-dependent-threshold-emission-angle-and-produced-photon-spectrum"></a>
![](cherenkov-dispersive-threshold-angle-yield.png)

**[Figure 11](#image-original-dispersive-cherenkov-radiation-model-a-wavelength-dependent-threshold-emission-angle-and-produced-photon-spectrum). Original dispersive Cherenkov radiation model: a wavelength-dependent threshold, emission angle, and produced photon spectrum**. All curves are calculations for the chosen finite-band [refractive index](refractive-index.md), with $z=1$ and $\alpha=1/137.036$. A missing angular segment means the threshold fails; the corresponding spectral yield is zero. The spectral axis is per centimetre of track and per nanometre of [vacuum](vacuum.md) [wavelength](wavelength.md), so it is $10^{-11}$ times the density in [SI](international-system-of-units.md) units. No historical observations, measured material constants, [absorption](absorption-electromagnetic-radiation.md) or detector response are plotted.

For a $1\,\mathrm{cm}$ track the chosen model predicts about $0.589$, $27.40$ and $142.85$ emitted [photons](photon.md) for $\beta=0.75$, $0.78$ and $0.90$, respectively. An expected count below one is meaningful over repeated equivalent tracks; it is not a fractional [photon](photon.md) observed on one track. The near-threshold example illustrates why extending a constant-index approximation across an entire optical band can give the wrong emitting interval.

Finite bandwidth is essential. The $1/\lambda^2$ factor cannot be extrapolated down to arbitrarily small [wavelength](wavelength.md): the chosen material model stops at its stated band. Real [optical dispersion](dispersion-optics.md) changes the threshold and direction, and appreciable [absorption](absorption-electromagnetic-radiation.md) requires a complex material response beyond the simple transparent-medium expression. A detected count must also include transport, collection geometry and the detector's wavelength-dependent response. Even a correct produced spectrum therefore does not, on its own, predict perceived colour or observed glow intensity.

## ↑ Ancestors (7)

1. [Frank-Tamm formula](frank-tamm-formula.md)
2. [Cherenkov radiation](cherenkov-radiation.md)
3. [Electromagnetic wave](electromagnetic-wave-split.md)
4. [Electromagnetism](electromagnetism-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Cherenkov radiation](cherenkov-radiation.md)
