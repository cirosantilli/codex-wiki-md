<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Fit radiatively corrected visible [cross sections](../../../../cross-section-physics.md) across the [Z boson](../../../../z-boson.md) [resonance](../../../../resonance.md). The line shape determines $M_Z$, the total [decay width](../../../../decay-width.md) $\Gamma_Z$, and pole normalizations

$$
\sigma_f^0=\frac{12\pi}{M_Z^2}\frac{\Gamma_e\Gamma_f}{\Gamma_Z^2}.
$$

The first extraction uses the fitted total and visible [partial decay widths](../../../../partial-decay-width.md). Assuming [lepton universality](../../../../lepton-universality.md), $\Gamma_e=\Gamma_\mu=\Gamma_\tau=\Gamma_\ell$, an absolute leptonic pole [cross section](../../../../cross-section-physics.md) gives $\Gamma_\ell=\Gamma_Z\sqrt{M_Z^2\sigma_\ell^0/(12\pi)}$. The hadronic-to-leptonic ratio gives $R_\ell=\Gamma_{\rm had}/\Gamma_\ell$. Subtracting every visible channel then yields

$$
\boxed{\Gamma_{\rm inv}=\Gamma_Z-\Gamma_{\rm had}-3\Gamma_\ell.}
$$

Without [lepton universality](../../../../lepton-universality.md), separately fitted visible leptonic widths replace $3\Gamma_\ell$, with sufficient independent information to disentangle their products with $\Gamma_e$.

A second, useful peak-normalization extraction first determines the invisible-to-leptonic ratio. Because

$$
\sigma_{\rm had}^0=\frac{12\pi}{M_Z^2}R_\ell\left(\frac{\Gamma_\ell}{\Gamma_Z}\right)^2,
$$

one obtains

$$
\boxed{R_{\rm inv}\equiv\frac{\Gamma_{\rm inv}}{\Gamma_\ell}=\sqrt{\frac{12\pi R_\ell}{M_Z^2\sigma_{\rm had}^0}}-R_\ell-3.}
$$

This ratio extraction does not require the measured line width. Multiplication by an independently predicted leptonic [partial decay width](../../../../partial-decay-width.md), or by $\Gamma_Z/(R_{\rm inv}+R_\ell+3)$ from the scan, converts it to $\Gamma_{\rm inv}$. Alternatively dividing $R_{\rm inv}$ by the predicted single-species ratio $\Gamma_\nu/\Gamma_\ell$ gives the number of light active [neutrinos](../../../../neutrino.md). These are two standard uses of line-shape information, with different choices of theoretical input; if both use the same fitted $\Gamma_\ell$, they are algebraically equivalent and statistically correlated, not independent determinations.

Statistical uncertainties in the reference-process counts give fluctuations in the [collider luminosity](../../../../collider-luminosity.md) at individual scan points, propagating into normalization and fitted line width. They decrease with additional reference events. A common multiplicative luminosity-scale systematic largely cancels in $R_\ell$ and the normalized line shape, but shifts every absolute peak [cross section](../../../../cross-section-physics.md). It therefore does not cancel from either invisible-width extraction. For a fractional upward luminosity shift $\varepsilon$, $\sigma_{\rm had}^0$ shifts by $-\varepsilon$, and at fixed $R_\ell,M_Z,\Gamma_Z$,

$$
\delta R_{\rm inv}\simeq\frac\varepsilon2(R_{\rm inv}+R_\ell+3),\qquad
\delta\Gamma_{\rm inv}\simeq\frac\varepsilon2(\Gamma_{\rm had}+3\Gamma_\ell).
$$

Thus overestimating luminosity increases the inferred invisible contribution. Energy-dependent systematic errors can also distort the line shape and its total [decay width](../../../../decay-width.md). The covariance matrix must retain correlations between scan points and experiments, including common theoretical uncertainty in the [Bhabha scattering](../../../../bhabha-scattering.md) calculation.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [6](../../6.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the particle physics course of the University of Oxford](../../../split.md)
5. [Particle physics course of the University of Oxford](../../../../particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
