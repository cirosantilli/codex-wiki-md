# ELODIE spectrograph

↑ **Parent:** [Doppler spectroscopy](doppler-spectroscopy.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/ELODIE_spectrograph)

Built by [André Baranne](andre-baranne.md), [Michel Mayor](michel-mayor.md), [Didier Queloz](didier-queloz.md) and colleagues, the ELODIE [fiber-fed spectrograph](fiber-fed-spectrograph.md) carried light from Haute-Provence's 1.93-metre telescope through [optical fibers](optical-fiber.md). Its [echelle grating](echelle-grating.md) dispersed light in high [diffraction orders](diffraction-order.md); an [optical prism](prism-optics.md) and [grism](grism.md) [cross-disperser](cross-disperser.md) separated them perpendicularly on a [charge-coupled device](charge-coupled-device.md). This [cross-dispersed echelle spectrograph](cross-dispersed-echelle-spectrograph.md) achieved [spectral resolving power](spectral-resolving-power.md) $R=42000$. A simultaneous [thorium](thorium.md) reference tracked [instrumental drift](instrumental-drift.md). [Wavelength calibration](wavelength-calibration.md) mapped detector positions to [wavelengths](wavelength.md); [spectral cross-correlation](spectral-cross-correlation.md) combined many [spectral lines](spectral-line.md) into a fitted profile. A [barycentric velocity correction](barycentric-velocity-correction.md) removed the observer's motion.[Baranne et al. (1996), abstract; section 3.1 and figure 6; section 3.7](elodie-a-spectrograph-for-accurate-radial-velocity-measurements-by-andre-baranne-and-others.md)

<a id="image-elodie-measurement-chain-and-synthetic-radial-velocity-readout"></a>
![](elodie-spectrum-to-radial-velocity.png)

**[Figure 3](#image-elodie-measurement-chain-and-synthetic-radial-velocity-readout). ELODIE measurement chain and synthetic radial-velocity readout**. Original schematic; the correlation profile and periodic signal are synthetic.

Why can a [spectrograph](spectrograph.md) measure a [Doppler shift](doppler-effect.md) much smaller than one [spectral resolution element](spectral-resolution-element.md)? Resolution concerns separating neighbouring features, whereas locating the centre of a known profile uses information across that profile and across many [spectral lines](spectral-line.md). For a chosen example, at $\lambda=500\,\mathrm{nm}$ a recession [velocity](velocity.md) of $60\,\mathrm{m\,s^{-1}}$ gives

$$
\Delta\lambda\simeq\lambda\frac{v_r}{c}=1.00069\times10^{-4}\,\mathrm{nm}.
$$

At $R=42000$, one [spectral resolution element](spectral-resolution-element.md) corresponds to $c/R\simeq7.14\,\mathrm{km\,s^{-1}}$, about $119$ times larger. A well measured centre can move by a small fraction of that width. More [photons](photon.md) and more useful [spectral lines](spectral-line.md) improve the estimate, but do not remove [wavelength calibration](wavelength-calibration.md) errors or [stellar activity](stellar-activity.md).

A simple mathematical picture of [spectral cross-correlation](spectral-cross-correlation.md) makes the readout concrete. Define $x=c\log(\lambda/\lambda_0)$, with fixed reference [wavelength](wavelength.md) $\lambda_0$, and let $d(x)$ be continuum-normalized line absorption. For small [velocities](velocity.md), a common [Doppler shift](doppler-effect.md) approximately translates $d(x)$. A positive absorption mask $m(x)$ then gives

$$
C(u)=\int d(x)m(x-u)\,dx.
$$

If $d(x)=m(x-v_r)$, the maximum occurs at $u=v_r$; a convention correlating the received [observed radiative flux](observed-radiative-flux.md) instead produces a dip. A fitted correlation centre is an effective collective line position, not a claim that each individual [spectral line](spectral-line.md) has been resolved into a narrower feature. The lamp tracks [instrumental drift](instrumental-drift.md), while the [barycentric velocity correction](barycentric-velocity-correction.md) removes the observer's changing line-of-sight [velocity](velocity.md); neither removes changes in the [star](star.md) itself.

## ↑ Ancestors (8)

1. [Doppler spectroscopy](doppler-spectroscopy.md)
2. [Exoplanet atmospheric observatory](exoplanet-atmospheric-observatory.md)
3. [Exoplanet atmosphere](exoplanet-atmosphere.md)
4. [Exoplanet](exoplanet-split.md)
5. [Astrophysics](astrophysics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)
