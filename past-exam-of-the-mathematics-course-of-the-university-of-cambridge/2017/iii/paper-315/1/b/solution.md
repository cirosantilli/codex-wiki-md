<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take $R_p$ to be the [radius](../../../../../../radius.md) of an opaque planetary disc and $H$ the geometric thickness of the model atmosphere, not necessarily one [atmospheric scale height](../../../../../../atmospheric-scale-height.md). Assume a uniform stellar [specific intensity](../../../../../../specific-intensity.md), a fully projected non-grazing transit, negligible planetary emission in the measured band, and no scattering or refraction returning light to the beam. The cylindrical approximation assigns the same slant [optical depth](../../../../../../optical-depth.md) $\tau_\lambda$ to every ray through the annulus.

The opaque disc blocks area $\pi R_p^2$. The annulus has projected area $\pi[(R_p+H)^2-R_p^2]$, and the [radiative transfer equation](../../../../../../radiative-transfer-equation.md) transmits fraction $e^{-\tau_\lambda}$ through it. Its blocked fraction is therefore $1-e^{-\tau_\lambda}$. Dividing the missing light by the unobscured stellar-disc light gives the [exoplanet transmission spectrum](../../../../../../exoplanet-transmission-spectrum.md)

$$
\boxed{D_\lambda=\frac{R_p^2+[(R_p+H)^2-R_p^2](1-e^{-\tau_\lambda})}{R_s^2}.}
$$

For $H\ll R_p$, the [annulus model for transmission spectroscopy](../../../../../../annulus-model-for-transmission-spectroscopy.md) becomes

$$
D_\lambda\simeq\left(\frac{R_p}{R_s}\right)^2
+\frac{2R_pH}{R_s^2}(1-e^{-\tau_\lambda}).
$$

The [optically thin](../../../../../../optically-thin-medium.md) excess is $2R_pH\tau_\lambda/R_s^2$; the [optically thick](../../../../../../optically-thick-medium.md) limit is the area ratio $(R_p+H)^2/R_s^2$ before the thin-annulus approximation. For a realistic atmosphere, the slant [optical depth](../../../../../../optical-depth.md) varies with the ray's impact parameter $b$, giving instead

$$
D_\lambda=\frac{R_p^2+2\int_{R_p}^{R_p+H}b[1-e^{-\tau_\lambda(b)}]\,db}{R_s^2}.
$$

[Limb darkening](../../../../../../limb-darkening.md) replaces the simple area weighting by the local stellar [specific intensity](../../../../../../specific-intensity.md). The constant-depth model is therefore an explicit geometric approximation, not the slant-depth law of a spherical hydrostatic atmosphere.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 315](../../../paper-315-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
