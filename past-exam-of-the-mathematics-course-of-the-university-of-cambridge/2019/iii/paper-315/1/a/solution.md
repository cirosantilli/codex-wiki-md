<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume a uniform stellar disc of radius $R_\star$, an opaque planetary radius $R_p$, and a thin atmospheric annulus of thickness $z\ll R_p$. Neglect planetary light during transit and scattering back into the beam. The attenuation part of the [radiative transfer equation](../../../../../../radiative-transfer-equation.md) gives $I_\lambda=I_{\lambda,0}e^{-\tau_\lambda}$, where $\tau_\lambda$ is the slant [optical depth](../../../../../../optical-depth.md) along a stellar ray through the atmosphere. The fraction of light removed from that annulus is therefore $1-e^{-\tau_\lambda}$.

If the annulus is represented by one effective [optical depth](../../../../../../optical-depth.md), its area divided by the stellar area is

$$
A=\frac{\pi[(R_p+z)^2-R_p^2]}{\pi R_\star^2}\simeq\frac{2R_pz}{R_\star^2}.
$$

The [annulus model for transmission spectroscopy](../../../../../../annulus-model-for-transmission-spectroscopy.md) consequently gives the extra transit depth

$$
\boxed{\delta_\lambda=A(1-e^{-\tau_\lambda}).}
$$

Here $\delta_\lambda$ is normalized to the unobscured stellar flux and excludes the opaque-disc depth $(R_p/R_\star)^2$. For a spectral feature measured relative to a continuum with slant [optical depth](../../../../../../optical-depth.md) $\tau_c$, the corresponding contrast is $A(e^{-\tau_c}-e^{-\tau_\lambda})$; the displayed formula takes the annular continuum to be transparent.

A real [exoplanet transmission spectrum](../../../../../../exoplanet-transmission-spectrum.md) has an impact-parameter-dependent [optical depth](../../../../../../optical-depth.md). Its more accurate expression is

$$
\delta_\lambda=\frac2{R_\star^2}\int_{R_p}^{\infty}b\,[1-e^{-\tau_\lambda(b)}],db.
$$

Stellar limb darkening and horizontally varying clouds further modify the weighting. The single-annulus approximation is useful for estimating an [atmospheric spectral-feature amplitude](../../../../../../atmospheric-spectral-feature-amplitude.md), rather than predicting every spectral line.

## ↑ Ancestors (11)

1. [A](../a.md)
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
