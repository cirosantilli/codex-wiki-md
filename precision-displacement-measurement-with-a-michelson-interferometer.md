# Precision displacement measurement with a Michelson interferometer

↑ **Parent:** [Michelson interferometer](michelson-interferometer.md)

A [Michelson interferometer](michelson-interferometer.md) turns [displacement](displacement.md) into a count of [interference fringes](interference-fringe.md): a moving mirror changes both the outward and return paths. This lets a [wavelength](wavelength.md) act as a ruler whose divisions need no engraving. Assume [normal incidence](normal-incidence.md), a fixed reference arm, stable [refractive index](refractive-index.md) $n$ along the moving arm, and fixed [vacuum](vacuum.md) [wavelength](wavelength.md) $\lambda_0$. Write $\lambda=\lambda_0/n$ for the [wavelength](wavelength.md) in that medium and take $\Delta L$ positive away from the [beam splitter](beam-splitter.md). The change in [optical path difference](optical-path-difference.md), the accumulated [phase difference](phase-difference.md), and the signed number of complete [interference fringe](interference-fringe.md) cycles are

$$
\Delta D=2n\Delta L,\qquad
\Delta\phi=\frac{2\pi\Delta D}{\lambda_0}=\frac{4\pi\Delta L}{\lambda},\qquad
\Delta N=\frac{\Delta\phi}{2\pi}=\frac{2\Delta L}{\lambda},\qquad
\Delta L=\frac{\lambda\Delta N}{2}.
$$

The factor two comes from propagation geometry: moving the mirror by $\Delta L$ adds $\Delta L$ before reflection and $\Delta L$ afterward. One bright-to-bright cycle means mirror travel $\lambda/2$; bright-to-dark means $\lambda/4$, half a cycle. All lengths must use compatible units, and $\Delta N$ is dimensionless. A constant reflection [phase difference](phase-difference.md) changes the initial fringe position but cancels from this change formula.

<a id="image-mirror-displacement-doubled-optical-path-difference-and-counted-interference-fringes-for-a-hypothetical-michelson-interferometer"></a>
![](michelson-mirror-displacement-fringe-count.png)

**[Figure 14](#image-mirror-displacement-doubled-optical-path-difference-and-counted-interference-fringes-for-a-hypothetical-michelson-interferometer). Mirror displacement, doubled optical path difference, and counted interference fringes for a hypothetical Michelson interferometer**.

For an original hypothetical example, suppose $\lambda=600\,\mathrm{nm}$ in the actual surrounding medium and a continuous scan gives $40.25$ cycles, including the final fractional cycle. Then $\Delta L=(600\,\mathrm{nm})(40.25)/2=12\,075\,\mathrm{nm}=12.075\,\mathrm{\mu m}$. With the [wavelength](wavelength.md) treated as exact, a fringe-reading [measurement uncertainty](measurement-uncertainty.md) of $0.02$ cycle contributes $6\,\mathrm{nm}$ to the [displacement](displacement.md) [measurement uncertainty](measurement-uncertainty.md). An uncertainty of $0.01\,\mathrm{rad}$ in a local [phase difference](phase-difference.md) instead corresponds to $600(0.01)/(4\pi)\,\mathrm{nm}\approx0.477\,\mathrm{nm}$. This illustrates [measurement resolution](measurement-resolution.md), not a complete claim of accuracy: [wavelength](wavelength.md) calibration, air changes, mirror tilt and missed cycles can dominate.

To separate the oscillating readout from its [optical coherence](optical-coherence.md) envelope, use the local model

$$
I(D)=\bar I\left[1+\mathcal V(D)\cos\left(\frac{2\pi D}{\lambda_0}+\phi_b\right)\right],
\qquad D=2(n_2L_2-n_1L_1).
$$

Here $I$ is detected [light intensity](light-intensity.md), $\bar I$ is the mean level, $\phi_b$ is a fixed bias [wave phase](phase-waves.md), and $\mathcal V$ is [interferometric visibility](interferometric-visibility.md). A fine scan of $D$ measures the carrier [phase difference](phase-difference.md); a coarse scan can map the [temporal optical coherence](temporal-optical-coherence.md) envelope through $\mathcal V(D)$. The envelope maximum locates matched delays only under the source and apparatus assumptions; it is not a bright fringe identifying an arbitrary mirror position. Even with known $\mathcal V$, one intensity reading leaves the [cosine](cosine.md) sign and whole-cycle ambiguities. Continuous motion of known direction, or an independently obtained pair of signals in [phase quadrature](phase-quadrature.md), is needed to recover signed travel through reversals.

<a id="image-proposed-michelson-interferometer-readout-and-hypothetical-optical-coherence-and-refractive-index-controls"></a>
![](michelson-displacement-coherence-controls.png)

**[Figure 15](#image-proposed-michelson-interferometer-readout-and-hypothetical-optical-coherence-and-refractive-index-controls). Proposed Michelson interferometer readout and hypothetical optical coherence and refractive index controls**.

The figure's original control example stipulates equal arm [light intensities](light-intensity.md), matching [linear polarizations](linear-polarization.md), and a Lorentzian [optical spectrum](optical-spectrum.md) giving $\mathcal V(D)=\exp(-|D|/L_c)$ with $L_c=1\,\mathrm{mm}$. In [vacuum](vacuum.md), arm mismatches $|L_2-L_1|=0.60\,\mathrm{mm}$ and $0.10\,\mathrm{mm}$ give $\mathcal V=e^{-1.2}\approx0.301$ and $e^{-0.2}\approx0.819$. Matching the arms improves the [phase difference](phase-difference.md) readout without changing its $\lambda_0/2$ travel per cycle. A fine mirror scan of one cycle changes $D$ by only $600\,\mathrm{nm}$ for the stipulated $600\,\mathrm{nm}$ source, much less than $L_c$. These are calculated values, not historical data.

A proposed measurement sequence follows from this model. Overlap the returning beams, match their [linear polarizations](linear-polarization.md), find a high-contrast delay and use a small calibrated mirror scan to determine the sign and fringe period. Read a fixed spatial sample of the [interference fringes](interference-fringe.md) with a [photodiode](photodiode.md); record each arm separately and the dark signal, avoid detector saturation, and retain enough time resolution to count every cycle. Approach mechanical settings consistently and repeat the return scan to expose lost motion or drift. For very small changes, bias near [phase quadrature](phase-quadrature.md), where $|dI/d\phi|=\bar I\mathcal V$ is largest; an intensity extremum has zero first-order sensitivity. A known drive voltage alone does not provide [measurement calibration](measurement-calibration.md) for mirror travel: compare the actual travel with the fringe count using an independently known [wavelength](wavelength.md).

Control [temperature](temperature-split.md), [pressure](pressure-split.md), vibration and air currents because the instrument measures [optical path difference](optical-path-difference.md), not mirror motion alone. For a fixed reference arm and fixed $\lambda_0$, the first-order change of the moving arm's round-trip path is $\Delta D\approx2n\Delta L+2L\Delta n$. Thus an unrecognized $\Delta n$ mimics $\Delta L_{\mathrm{app}}=L\Delta n/n$. A hypothetical $L=0.10\,\mathrm m$, $n\approx1$, and $\Delta n=10^{-7}$ give $10\,\mathrm{nm}$ apparent travel. Holding the mirror still while varying or monitoring the air conditions tests this confounder. Separate checks of alignment, [wavelength](wavelength.md) stability and [thermal expansion](thermal-expansion.md) are necessary before sub-fringe [measurement resolution](measurement-resolution.md) becomes a defensible [measurement uncertainty](measurement-uncertainty.md).

## ↑ Ancestors (9)

1. [Michelson interferometer](michelson-interferometer.md)
2. [Temporal optical coherence](temporal-optical-coherence.md)
3. [First-order optical coherence](first-order-optical-coherence.md)
4. [Optical coherence](optical-coherence.md)
5. [Physical optics](physical-optics-split.md)
6. [Optics](optics-split.md)
7. [Branches of physics](branches-of-physics.md)
8. [Physics](physics-split.md)
9. [Codex Wiki](split.md)
