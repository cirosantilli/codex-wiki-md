<h1 id="6/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

[Fluorescence localization precision](../../../../fluorescence-localization-precision.md) can be much finer than the image width: a fluorescent [molecule](../../../../molecule-split.md) produces a [diffraction](../../../../diffraction.md)-broadened [point spread function](../../../../point-spread-function-split.md), but the centre of that distribution can be estimated much more precisely than its width. Fit the measured camera counts to a calibrated point-spread model with position, brightness and background parameters. For an ideal [Gaussian](../../../../gaussian-function.md) image of [standard deviation](../../../../standard-deviation.md) $s$ and $N$ independent detected [photons](../../../../photon.md), the centroid precision scales as

$$
\boxed{\sigma_{\rm loc}\simeq\frac{s}{\sqrt N}.}
$$

Pixelation and background worsen this limit. A useful approximate [variance](../../../../variance-split.md) for square pixels of width $a$ and background rms noise $b$ [photons](../../../../photon.md) per pixel is

$$
\sigma_{\rm loc}^2\simeq\frac{s^2+a^2/12}{N}+\frac{8\pi s^4b^2}{a^2N^2}.
$$

This estimate requires a correctly specified isolated image and appropriate noise model. Drift, optical aberration, dye motion, linkage offset, [bleaching](../../../../photobleaching.md) and [motion blur](../../../../motion-blur.md) introduce further errors; localization precision alone does not guarantee absolute positional accuracy.[Photon number, pixel size and background dependence of localization uncertainty](../../../../precise-nanometer-localization-analysis-for-individual-fluorescent-probes-by-russell-e-thompson-and-others.md)

In the [Myosin V](../../../../myosin-v.md) measurements, [total internal reflection fluorescence microscopy](../../../../total-internal-reflection-fluorescence-microscopy.md) reduced background and a two-dimensional [Gaussian](../../../../gaussian-function.md) fit localized a single dye attached to a light chain with roughly $1.5\,\mathrm{nm}$ precision. The motor's centre advances about $37\,\mathrm{nm}$ per cycle. A [hand-over-hand mechanism](../../../../hand-over-hand-motion-of-a-two-headed-motor.md) instead moves the rear head about $74\,\mathrm{nm}$ past the stationary front head, exchanging their roles. A label displaced by $x$ from the midpoint therefore gives alternating displacements $37+2x$ and $37-2x$ nm; near a head this tends towards alternating $74$ and $0$ nm. An [inchworm model](../../../../inchworm-motion-of-a-two-headed-motor.md) would give approximately uniform $37$ nm label displacements. Resolved unequal alternating steps therefore distinguish the mechanisms, with interpretation depending on the label geometry.[Single-light-chain fluorophore localization, alternating displacements and hand-over-hand interpretation; Science 300, 2061–2065 (2003)](../../../../myosin-v-walks-hand-over-hand-single-fluorophore-imaging-with-1-5-nm-localization-by-ahmet-yildiz-and-others.md)

For sub-[diffraction](../../../../diffraction.md) imaging, arrange that only a sparse, spatially separable subset of [fluorophores](../../../../fluorophore.md) emits in each frame, localize those emitters, then combine many frames into a map. Photoactivation or reversible stochastic switching provides the sparse subsets. Distinct nearby [molecules](../../../../molecule-split.md) can then be localized at different times, circumventing overlap of their simultaneously emitted [diffraction](../../../../diffraction.md) patterns. The achievable structural resolution depends on [photon](../../../../photon.md)-limited precision, label density and linkage, repeated blinking, drift correction and specimen motion; arbitrarily many fits to the same dye do not supply missing labels elsewhere. This is the principle behind [PALM](../../../../photoactivated-localization-microscopy.md) and [STORM](../../../../stochastic-optical-reconstruction-microscopy.md), with their different switching strategies.[Sequential sparse activation and localization of fluorophores to reconstruct a super-resolution image](../../../../sub-diffraction-limit-imaging-by-stochastic-optical-reconstruction-microscopy-storm-by-michael-j-rust-and-others.md)

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [6](../../6.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
