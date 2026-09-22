# X-ray attenuation

↑ **Parent:** [X-ray](x-ray.md)

For a narrow beam of monoenergetic [photons](photon.md) crossing homogeneous material of thickness $x$, the uncollided [wave intensity](intensity-physics.md) obeys $I(x)=I_0e^{-\mu x}$. Here $\mu$ is the [linear attenuation coefficient](linear-attenuation-coefficient.md), counting removal from the incident beam by [photon absorption](photon-absorption.md) and [scattering of light](scattering-of-light.md). It depends on [photon](photon.md) [energy](energy-split.md) and material; it is not universally independent of [energy](energy-split.md).[Tables of X-Ray Mass Attenuation Coefficients and Mass Energy-Absorption Coefficients by John H. Hubbell and Stephen M. Seltzer; NIST, X-Ray Mass Attenuation Coefficients, §2, Eq. (1), narrow monoenergetic beam and interaction contributions](tables-of-x-ray-mass-attenuation-coefficients-and-mass-energy-absorption-coefficients-by-john-h-hubbell-and-stephen-m-seltzer/2-the-mass-attenuation-coefficient.md)

An original derivation makes the model explicit. If each thin layer removes fraction $\mu\,dx$ of the surviving beam, with the same $\mu$ throughout, then

$$
\frac{dI}{dx}=-\mu I,\qquad
\ln\frac{I(x)}{I_0}=-\mu x.
$$

Thus equal added thicknesses multiply transmission by the same factor. The [ordinary differential equation](ordinary-differential-equation.md) describes uncollided beam survival. To test it with a detector, keep source output, distance, selected [photon](photon.md) [energy](energy-split.md) band and detector response fixed. Use a [collimator](collimator.md) and suitable detector acceptance to exclude [scattering of light](scattering-of-light.md) into the detector. Subtract background, measure an empty-path reference, and keep the detector in its linear operating range. A changing source distance adds geometric dilution and is not an attenuation measurement at fixed geometry.

For a stipulated example, take $\mu=0.40\,\mathrm{mm^{-1}}$ and $x=2.5\,\mathrm{mm}$. Transmission is $e^{-1}\simeq0.368$. If the empty-path detector rate is $1010\,\mathrm{s^{-1}}$, including background $b=10\,\mathrm{s^{-1}}$, the model predicts sample rate $10+1000e^{-1}\simeq378\,\mathrm{s^{-1}}$. Recover transmission as $(R-b)/(R_0-b)$; the raw ratio $R/R_0\simeq0.374$ is biased. These chosen values are a calculation, not measurements of a particular material or a historical apparatus.

<a id="image-x-ray-narrow-beam-attenuation"></a>
![](x-ray-narrow-beam-attenuation.png)

**[Figure 10](#image-x-ray-narrow-beam-attenuation). When X-ray transmission is exponential, and when spectral mixing bends it**. Original calculated examples, with stipulated [linear attenuation coefficients](linear-attenuation-coefficient.md) in inverse millimetres. The left panel uses one [photon](photon.md) [energy](energy-split.md) and marks $x=2.5\,\mathrm{mm}$ and the [half-value layer](half-value-layer.md). The right panel compares an equal-weight mixture of two [photon](photon.md) [energies](energy-split.md) with the exponential having the same initial slope. A logarithmic vertical axis turns a single exponential into a straight line. Neither curve is fitted to measured material data.

**Table of contents**

- [Linear attenuation coefficient](linear-attenuation-coefficient.md)
  - [Linear energy-absorption coefficient](linear-energy-absorption-coefficient.md)
  - [Exponential attenuation](exponential-attenuation.md)
  - [Mass attenuation coefficient](mass-attenuation-coefficient.md)
- [Half-value layer](half-value-layer.md)
- [Beam hardening](beam-hardening.md)
- [Absorption edge](absorption-edge.md)

## ↑ Ancestors (6)

1. [X-ray](x-ray.md)
2. [Electromagnetic radiation](electromagnetic-radiation-split.md)
3. [Electromagnetism](electromagnetism-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Crystal X-ray spectrometer](crystal-x-ray-spectrometer.md)
- [Röntgen X-ray discovery experiment](rontgen-x-ray-discovery-experiment.md)
