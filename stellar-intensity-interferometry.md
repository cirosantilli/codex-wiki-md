# Stellar intensity interferometry

↑ **Parent:** [Hanbury Brown and Twiss effect](hanbury-brown-and-twiss-effect.md)

[Stellar intensity interferometry](stellar-intensity-interferometry.md) measures a [star](star.md)'s [angular diameter](angular-diameter.md) by comparing fluctuations of detected [light intensity](light-intensity.md) at separated collectors. Each collector has its own [photodetector](photodetector.md); an [analog multiplier](analog-multiplier.md) or a digital correlator compares the electrical outputs. Changing the [interferometric baseline](interferometric-baseline.md) changes the sampled [spatial optical coherence](spatial-optical-coherence.md). An unresolved [star](star.md) produces correlated fluctuations; a resolved extended source supplies different mixtures of emission directions, reducing their correlation.

This makes a useful telescope out of a surprising observable: the fluctuations discarded by an ordinary average-brightness measurement. Optical beams need not travel to a common combiner. A relative [wave phase](phase-waves.md) perturbation $E_2\mapsto e^{i\phi}E_2$ leaves $|E_2|^2$ unchanged, so pure phase errors do not directly change the local [light intensity](light-intensity.md). Electronic delay alignment remains necessary; intensity changes from [atmospheric scintillation](scintillation-astronomy.md), collection losses, and instrumental noise still require controls.

Let $\mathbf b$ join the collectors and let $\mathbf s_0$ be the unit [line of sight](line-of-sight.md) toward the [star](star.md). The relevant [interferometric baseline](interferometric-baseline.md) is its projection onto the [plane of the sky](plane-of-the-sky.md):

$$
\mathbf b_\perp=\mathbf b-(\mathbf b\cdot\mathbf s_0)\mathbf s_0,
\qquad B=|\mathbf b_\perp|.
$$

The reference arrival-time difference has magnitude $|\mathbf b\cdot\mathbf s_0|/c$, with [speed of light](speed-of-light.md) $c$. Correct that delay, with a sign fixed by channel order, before averaging the residual correlation at $\tau=0$. The physical collector separation equals $B$ only when it is perpendicular to $\mathbf s_0$; tracking a [star](star.md) can change the projection even for fixed collectors.

<a id="image-functional-geometry-of-stellar-intensity-interferometry-separate-optical-detection-followed-by-electrical-correlation"></a>
![](stellar-intensity-interferometer-geometry.png)

**[Figure 3](#image-functional-geometry-of-stellar-intensity-interferometry-separate-optical-detection-followed-by-electrical-correlation). Functional geometry of stellar intensity interferometry: separate optical detection followed by electrical correlation**. Original schematic with the reference direction normal to the baseline. Matched optical selection feeds independent detectors; mean removal, response and delay alignment precede multiplication and averaging. This is not a scale drawing of the historical apparatus.

**Table of contents**

- [Sirius intensity interferometry experiment](sirius-intensity-interferometry-experiment.md)
- [Siegert relation](siegert-relation.md)
- [Uniform-disk stellar visibility](uniform-disk-stellar-visibility.md)
  - [Stellar angular diameter from a visibility envelope](stellar-angular-diameter-from-a-visibility-envelope.md)
- [Finite-response stellar intensity correlations](finite-response-stellar-intensity-correlations.md)

## ↑ Ancestors (6)

1. [Hanbury Brown and Twiss effect](hanbury-brown-and-twiss-effect.md)
2. [Quantum optics](quantum-optics-split.md)
3. [Quantum theory](quantum-theory-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-frontiers-of-observational-astrophysics-course-of-the-university-of-cambridge/2014/paper-1/3/b/solution.md)
- [Siegert relation](siegert-relation.md)
- [Stellar intensity interferometry](stellar-intensity-interferometry.md)
