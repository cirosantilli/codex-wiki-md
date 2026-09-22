<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

**Position from many photons.** An isolated [fluorophore](../../../../fluorophore.md) produces a diffraction-broadened [point spread function](../../../../point-spread-function-split.md), but its unknown center can be inferred much more precisely than the width of that function. Fit a calibrated two-dimensional [Gaussian function](../../../../gaussian-function.md) plus background to the detected photon positions or pixel intensities. If the [point spread function](../../../../point-spread-function-split.md) has width $s$ and $N_\gamma$ independent photons are detected, negligible background gives [localization precision](../../../../localization-precision.md) approximately $s/\sqrt{N_\gamma}$. Pixelation and background worsen it; a commonly useful approximate [variance](../../../../variance-split.md) is

$$
\sigma_x^2\simeq\frac{s^2+a^2/12}{N_\gamma}
+\frac{8\pi s^4\sigma_{\rm bg}^2}{a^2N_\gamma^2},
$$

where $a$ is pixel size in the specimen plane and $\sigma_{\rm bg}$ is background noise per pixel in photon units. Bright, isolated emitters can therefore have nanometre [localization precision](../../../../localization-precision.md) despite a spot hundreds of nanometres wide. Stage drift, finite exposure motion, incorrect fitting, label displacement and [photobleaching](../../../../photobleaching.md) can dominate the photon limit.[Localization-error analysis: photon number, pixel size and background contributions](../../../../precise-nanometer-localization-analysis-for-individual-fluorescent-probes-by-russell-e-thompson-and-others.md)

**Walking mechanism.** [Myosin V](../../../../myosin-v.md) is a two-headed, processive [molecular motor](../../../../molecular-motor.md) that advances along [actin](../../../../actin.md) with center-of-mass steps of about $37\,\mathrm{nm}$. A simple inchworm model retains the identity of the leading head, so a label fixed to one head would move approximately $37\,\mathrm{nm}$ on every cycle. In a hand-over-hand model the heads exchange lead: a label close to one head alternates a displacement near $74\,\mathrm{nm}$ with a near-zero displacement while the other head passes. For a label at offset $x$ from the midpoint, the more general alternating pair is $37-2x$ and $37+2x$ nanometres. The pair sums to $74\,\mathrm{nm}$; individual steps need not always equal $74\,\mathrm{nm}$.

Single-label imaging records a moving spot on a camera while the motor travels along surface-associated [actin](../../../../actin.md). Fitting the spot in successive frames resolves plateaus and jumps much smaller than the diffraction width. The observed alternating displacements distinguish a passing-head mechanism from uniform inchworm steps. This experiment combines a specific geometric prediction with [single-molecule fluorescence microscopy](../../../../single-molecule-fluorescence-microscopy.md); the center-of-mass stride alone would not make that distinction.[Science 300, pp. 2061–2065: single-label tracking, 1.5-nm localization and alternating displacement predictions](../../../../myosin-v-walks-hand-over-hand-single-fluorophore-imaging-with-1-5-nm-localization-by-ahmet-yildiz-and-others.md)

**Resolving a labelled structure.** Accurate localization of one emitter does not automatically resolve two simultaneously overlapping emitters. [Stochastic optical reconstruction microscopy](../../../../stochastic-optical-reconstruction-microscopy.md) overcomes this by activating or switching on only a sparse subset at a time, localizing the well-separated spots, turning them off and repeating. The accumulated coordinates reconstruct a densely labelled structure at scales below the diffraction limit. The original demonstration used repeated photoswitching and localization of individual dyes to reconstruct subdiffraction features.[Nature Methods 3, pp. 793–796: sequential localization of photoswitchable fluorophores](../../../../sub-diffraction-limit-imaging-by-stochastic-optical-reconstruction-microscopy-storm-by-michael-j-rust-and-others.md)

The useful structural resolution depends on both [localization precision](../../../../localization-precision.md) and label sampling density, as well as drift, fluorophore blinking, optical aberrations and linkage error. Sparse activation separates emitters in time; it does not shrink the diffraction-limited [point spread function](../../../../point-spread-function-split.md). A reconstructed image must have enough independent labels to represent its finest claimed feature.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [6](../../6.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
