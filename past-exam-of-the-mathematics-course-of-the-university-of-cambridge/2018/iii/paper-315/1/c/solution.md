<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume that the optical continuum is dominated by [Rayleigh scattering](../../../../../../rayleigh-scattering.md) by particles much smaller than the wavelength, and that their column abundance is fixed. Their cross-section, hence the slant [optical depth](../../../../../../optical-depth.md), scales as $\tau_\lambda\propto\lambda^{-4}$. Differentiating the [annulus model for transmission spectroscopy](../../../../../../annulus-model-for-transmission-spectroscopy.md) exactly gives the [logarithmic slope of total transit depth](../../../../../../logarithmic-slope-of-total-transit-depth.md)

$$
\boxed{\frac{d\ln\delta_\lambda}{d\ln\lambda}
=-4\frac{B\tau_\lambda e^{-\tau_\lambda}}{A+B(1-e^{-\tau_\lambda})}}.
$$

For $A\geq0$ and $B>0$, the slope lies between $-4$ and zero, but generally depends on wavelength. In the [optically thin](../../../../../../optically-thin-medium.md) limit, $\delta_\lambda\simeq A+B\tau_\lambda$, so its slope is $-4B\tau_\lambda/(A+B\tau_\lambda)$. It vanishes as the atmospheric signal becomes negligible compared with the opaque disc; it also approaches zero in the saturated [optically thick](../../../../../../optically-thick-medium.md) limit.

The familiar value $m\simeq-4$ applies to the [optically thin](../../../../../../optically-thin-medium.md) atmospheric excess,

$$
\boxed{\frac{d\ln(\delta_\lambda-A)}{d\ln\lambda}\simeq-4},
$$

or formally to a model in which $A$ is negligible. For an ordinary thin [exoplanet atmosphere](../../../../../../exoplanet-atmosphere.md), however, $B/A\simeq2H/R_p\ll1$, so neglecting the opaque planetary baseline in the total transit depth is not usually justified. **A universal $m=-4$ for the logarithm of the total transit depth does not follow from the stated model.**

In a stratified [isothermal atmosphere](../../../../../../isothermal-atmosphere.md), the related [scattering slope of a transmission spectrum](../../../../../../scattering-slope-of-a-transmission-spectrum.md) is instead $dR_{\rm tr}/d\ln\lambda=-4h$, obtained by moving the effective tangent level to keep its slant [optical depth](../../../../../../optical-depth.md) of order unity. Consequently $d\ln\delta/d\ln\lambda=-8h/R_{\rm tr}$ there. The radius slope, atmospheric-excess slope and total-depth slope are different observables.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 315](../../../paper-315-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
