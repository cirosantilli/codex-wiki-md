<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In the [annulus model for transmission spectroscopy](../../../../../../annulus-model-for-transmission-spectroscopy.md), an added aerosol [optical depth](../../../../../../optical-depth.md) changes the signal to $A[1-e^{-(\tau_{\rm gas}+\tau_{\rm aerosol})}]$. Large particles can supply nearly wavelength-independent extinction. An opaque high [exoplanet cloud deck](../../../../../../exoplanet-cloud-deck.md) then masks deeper gas, flattens the optical [exoplanet transmission spectrum](../../../../../../exoplanet-transmission-spectrum.md), and weakens atomic or molecular features.

Small particles can instead produce a rising transit radius toward short wavelengths. In an isothermal atmosphere, the [slant optical depth of an isothermal atmosphere](../../../../../../slant-optical-depth-of-an-isothermal-atmosphere.md) is

$$
\tau_\lambda(z)\simeq\sigma_\lambda n_0e^{-z/H}\sqrt{2\pi R_pH}.
$$

Taking the effective radius near $\tau_\lambda\sim1$ gives $z(\lambda)=H\log\sigma_\lambda+\mathrm{constant}$. For [Rayleigh scattering](../../../../../../rayleigh-scattering.md), $\sigma_\lambda\propto\lambda^{-4}$, so the [scattering slope of a transmission spectrum](../../../../../../scattering-slope-of-a-transmission-spectrum.md) is

$$
\boxed{\frac{dR_p}{d\log\lambda}=-4H.}
$$

A steeper-than-expected optical slope or suppressed gas features can therefore indicate [atmospheric haze](../../../../../../haze.md) or [exoplanet clouds](../../../../../../exoplanet-cloud.md). These signatures are not unique: high mean molecular mass reduces $H$, gas itself can produce [Rayleigh scattering](../../../../../../rayleigh-scattering.md), and stellar surface heterogeneity can mimic slopes. Consistent optical and infrared features help distinguish these explanations.

## ↑ Ancestors (11)

1. [C](../c.md)
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
