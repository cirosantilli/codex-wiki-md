<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

At 10 parsecs, $0.01$ arcseconds corresponds to $a=0.10$ astronomical units. Take a solar-radius star with $T_\star=5772\,\mathrm K$, zero [Bond albedo](../../../../../../bond-albedo.md), full [day-night heat redistribution](../../../../../../day-night-heat-redistribution.md), negligible internal heating, and a hydrogen-helium atmosphere with mean particle mass $2.3m_H$. The [planetary equilibrium temperature](../../../../../../planetary-equilibrium-temperature.md) is

$$
T_p=T_\star\sqrt{\frac{R_\star}{2a}}\simeq880\,\mathrm K.
$$

For [Jupiter](../../../../../../jupiter.md) mass and radius, $g\simeq24.8\,\mathrm{m\,s^{-2}}$. Its [atmospheric scale height](../../../../../../atmospheric-scale-height.md) is

$$
H=\frac{k_BT_p}{2.3m_Hg}\simeq1.27\times10^5\,\mathrm m.
$$

Assume a strong band spans $N_H=5$ [atmospheric scale heights](../../../../../../atmospheric-scale-height.md) and saturates in the [annulus model for transmission spectroscopy](../../../../../../annulus-model-for-transmission-spectroscopy.md). The [atmospheric spectral-feature amplitude](../../../../../../atmospheric-spectral-feature-amplitude.md) is

$$
\delta_{\rm tr}\simeq\frac{2R_pN_HH}{R_\star^2}\simeq1.88\times10^{-4}=188\,\mathrm{ppm}.
$$

For a five-standard-deviation detection, the uncertainty of the measured differential contrast must satisfy

$$
\boxed{\sigma_{\rm tr}\lesssim38\,\mathrm{ppm}.}
$$

This estimate scales linearly with the assumed feature height; one [atmospheric scale height](../../../../../../atmospheric-scale-height.md) would require about $7.5\,\mathrm{ppm}$. The question gives no opacity or abundance from which to fix $N_H$, so an atmospheric detection threshold is necessarily assumption-dependent.

For thermal emission at $10\,\mu\mathrm m$, assume the planet and star emit as [blackbodies](../../../../../../blackbody.md). The [thermal eclipse depth](../../../../../../thermal-eclipse-depth.md) from the [Planck law](../../../../../../planck-s-law.md) is

$$
\frac{F_p}{F_\star}=\left(\frac{R_p}{R_\star}\right)^2
\frac{e^{hc/(\lambda k_BT_\star)}-1}{e^{hc/(\lambda k_BT_p)}-1}
\simeq7.24\times10^{-4}=724\,\mathrm{ppm}.
$$

Thus the uncertainty required for a five-standard-deviation [exoplanet secondary eclipse](../../../../../../exoplanet-secondary-eclipse.md) detection is

$$
\boxed{\sigma_{\rm em}\lesssim145\,\mathrm{ppm}.}
$$

These are uncertainties of the final transit or eclipse contrasts, including the uncertainty of their reference levels. The distance affects photon counts and observing time but cancels from the flux ratios. An opaque exactly isothermal atmosphere emits a featureless [blackbody](../../../../../../blackbody.md) spectrum: an eclipse detects its thermal light, while identifying atmospheric composition requires spectral features and a nonisothermal structure or other diagnostics.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 315](../../../paper-315-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
