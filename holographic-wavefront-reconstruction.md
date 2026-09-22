# Holographic wavefront reconstruction

↑ **Parent:** [Holography](holography.md)

Take stationary scalar [monochromatic waves](monochromatic-wave.md) of the same [frequency](frequency.md) and [polarization of an electromagnetic wave](polarization-of-an-electromagnetic-wave.md), with time convention $e^{-i\omega t}$. Write their [complex amplitudes](complex-amplitude.md) at the recording plane as $R=A_R e^{i\phi_R}$ and $O=A_O e^{i\phi_O}$, absorbing the common conversion to [irradiance](irradiance.md) into the units. An exposure short enough to avoid fringe motion but long compared with an optical period records

$$
I=|R+O|^2=|R|^2+|O|^2+R^*O+RO^*
=A_R^2+A_O^2+2A_RA_O\cos(\phi_O-\phi_R).
$$

The two cross terms are where relative [wave phase](phase-waves.md) enters the measured [light intensity](light-intensity.md). Blocking the [holographic reference wave](holographic-reference-wave.md) leaves $|O|^2$ and removes them. Loss of mutual [optical coherence](optical-coherence.md), incompatible [polarization of an electromagnetic wave](polarization-of-an-electromagnetic-wave.md) or motion that averages the relative [wave phase](phase-waves.md) similarly reduces fringe contrast. These are useful controls for distinguishing a [hologram](hologram.md) from an ordinary brightness record. One local cosine value does not uniquely determine a [wave phase](phase-waves.md); known reference structure and separation of the cross terms supply the additional information in the example below.

Model a thin weakly modulated recording by its [amplitude transmittance](amplitude-transmittance.md)

$$
t=t_0+\beta I,\qquad |\beta I|\ll|t_0|.
$$

Here $t_0$ and $\beta$ are real constants in a local linear response to exposure at a fixed exposure time. They describe a chosen [amplitude modulation](amplitude-modulation.md) model, not a universal photographic response; an absorbing negative may have $\beta<0$. Keep $0\leq t\leq1$ for this passive real-transmission model. Ignore material thickness, saturation, shrinking, clipping and changes of [wavelength](wavelength.md). Illuminating the processed record with the original $R$ gives, immediately after the plate,

$$
Rt=\underbrace{\bigl[t_0+\beta(|R|^2+|O|^2)\bigr]R}_{\text{zero-order background}}
+\underbrace{\beta|R|^2O}_{\text{desired object field}}
+\underbrace{\beta R^2O^*}_{\text{conjugate field}}.
$$

This follows by multiplying the preceding identity by $R$; no [wave phase](phase-waves.md) detector has been assumed. If $|R|$ is uniform, the desired term reproduces $O$ up to a constant. A nonuniform $|R|^2$ weights the recovered field. With a strong [holographic reference wave](holographic-reference-wave.md), the $|O|^2R$ contamination is small relative to $|R|^2R$, but it is retained in this identity. Subsequent [diffraction](diffraction.md) propagates each term: reproduction at the plate is the starting boundary field, not yet a focused image.

<a id="image-recording-light-intensity-and-reconstructing-wavefronts-original-functional-geometry-for-in-line-holography"></a>
![](holography-recording-and-reconstruction-geometry.png)

**[Figure 19](#image-recording-light-intensity-and-reconstructing-wavefronts-original-functional-geometry-for-in-line-holography). Recording light intensity and reconstructing wavefronts: original functional geometry for in-line holography**.

The schematic uses a [plane wave](plane-wave.md) reference and one [optical point source](optical-point-source.md) to separate the functions. The top row records $R+O$; the bottom removes the object and illuminates the developed [hologram](hologram.md) with $R$. Dashed extensions identify the desired [virtual image](virtual-image.md); the conjugate component converges toward a [real image](real-image.md). All three outgoing components coexist. The coloured paths distinguish terms, not different [wavelengths](wavelength.md); distances and strengths are schematic. This functional drawing is not a reconstruction of the historical apparatus.

## ↑ Ancestors (6)

1. [Holography](holography.md)
2. [Physical optics](physical-optics-split.md)
3. [Optics](optics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Hologram](hologram.md)
