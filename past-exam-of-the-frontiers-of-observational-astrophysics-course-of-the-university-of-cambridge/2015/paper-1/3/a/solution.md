<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

**[Stellar reflex motion](../../../../../stellar-reflex-motion.md).** A [planet](../../../../../planet.md) and its host orbit their common [barycentre](../../../../../barycenter.md). The [star](../../../../../star.md)'s line-of-sight velocity shifts its [absorption lines](../../../../../absorption-line.md) by $\Delta\lambda/\lambda\simeq v_r/c$ at low speeds. A time series can be fitted with

$$
v_r(t)=\gamma+K[\cos(\nu(t)+\varpi)+e\cos\varpi],\qquad
K=\left(\frac{2\pi G}{P}\right)^{1/3}
\frac{M_p\sin i}{(M_\star+M_p)^{2/3}\sqrt{1-e^2}}.
$$

Here $\nu(t)$ is [true anomaly](../../../../../true-anomaly.md), $\varpi$ the argument of periastron and $\gamma$ an arbitrary systemic velocity offset. At small companion mass and known stellar mass, the orbit supplies $M_p\sin i$, not the true [planet](../../../../../planet.md) mass without an inclination constraint. Long monitoring helps distinguish a reproducible Keplerian signal from stellar oscillations, magnetic activity, spots and instrumental trends.

**The Lick reference-cell implementation.** Starlight passes through a temperature-controlled cell of molecular [iodine](../../../../../iodine.md) before entering the Hamilton high-resolution echelle [spectrograph](../../../../../spectrograph.md). The cell imprints a dense pattern of reference [absorption lines](../../../../../absorption-line.md) on the stellar spectrum, predominantly in the approximately $500$–$630\ {\rm nm}$ interval. These lines share the same exposure and downstream optical path as the stellar light. A calibrated high-resolution Fourier-transform [iodine](../../../../../iodine.md) spectrum and an iodine-free stellar template allow the [wavelength](../../../../../wavelength.md) solution and instrumental line-spread function to be fitted along with the stellar [Doppler shift](../../../../../doppler-effect.md). The method corrects shifts and line-shape changes that a separate [calibration](../../../../../calibration-differential-geometry.md) exposure would not necessarily follow.[Marcy and Butler (1992), sections 3–4, printed pages 271–274: Hamilton setup, iodine wavelength interval, templates and in-situ instrumental profile](../../../../../precision-radial-velocities-with-an-iodine-absorption-cell-by-geoffrey-w-marcy-and-r-paul-butler.md)

A useful forward model for one short spectral segment is

$$
\boxed{f_{\rm obs}(\lambda)=
\left\{S\!\left(\frac{\lambda}{1+v/c}\right)T_{\rm I_2}(\lambda)\right\}
*\mathcal P(\lambda),}
$$

followed by pixel integration, continuum scaling and a fitted [wavelength](../../../../../wavelength.md) [calibration](../../../../../calibration-differential-geometry.md). Here $S$ is the intrinsic stellar spectrum, $T_{\rm I_2}$ the cell transmission and $\mathcal P$ the instrumental line-spread function. The spectra multiply before [convolution](../../../../../convolution.md); simply dividing a recorded blended spectrum by the laboratory [iodine](../../../../../iodine.md) spectrum is not equivalent to this model. The [iodine](../../../../../iodine.md) pattern is stationary in the observatory frame while stellar lines move relative to it. Separate spectral segments accommodate [wavelength](../../../../../wavelength.md) dependence of the instrumental profile.

<a id="3/a/image-original-synthetic-iodine-cell-forward-model-showing-multiplication-before-instrumental-convolution-all-line-positions-and-strengths-are-illustrative"></a>
![](../../../../../past-exam-of-the-frontiers-of-observational-astrophysics-course-of-the-university-of-cambridge/2015/paper-1-iodine-forward-model.png)

**[Figure 3](#3/a/image-original-synthetic-iodine-cell-forward-model-showing-multiplication-before-instrumental-convolution-all-line-positions-and-strengths-are-illustrative). Original synthetic iodine-cell forward model showing multiplication before instrumental convolution; all line positions and strengths are illustrative**.

Earth's rotational and orbital velocities must then be removed with a barycentric correction using accurate timing, ideally weighted by [photon](../../../../../photon.md) arrival rate. Many stellar lines constrain a shift smaller than one instrumental resolution element; spectral resolution alone is not the velocity error. [Photon](../../../../../photon.md) statistics, template quality, instrumental-profile modelling and intrinsic stellar variability limit the precision. The method measures changes relative to a template and does not by itself provide a perfectly absolute centre-of-mass velocity. No particular discovery, modern precision floor or historical observing performance is assumed here.

## ↑ Ancestors (14)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the frontiers of Observational Astrophysics course of the University of Cambridge](../../../../split.md)
6. [Frontiers of Observational Astrophysics course of the University of Cambridge](../../../../../frontiers-of-observational-astrophysics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
