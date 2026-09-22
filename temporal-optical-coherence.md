# Temporal optical coherence

↑ **Parent:** [First-order optical coherence](first-order-optical-coherence.md)

[Temporal optical coherence](temporal-optical-coherence.md) compares a field at one position with a delayed copy. In a [Michelson interferometer](michelson-interferometer.md), unequal round-trip lengths supply this delay. Even a source with rapidly changing [wave phase](phase-waves.md) can give high [interferometric visibility](interferometric-visibility.md) close to zero delay, because both arms then deliver nearly the same source history. A source narrowed in [optical spectrum](optical-spectrum.md) generally retains correlation over larger delays; a single width does not describe sources with several separated lines. [MIT 2.71/2.710, lecture 22, slides 2–5: temporal and spatial coherence](https://ocw.mit.edu/courses/2-71-optics-spring-2009/bebe78c6a2ae2603a0d1a3ea85e0b4ca_MIT2_71S09_lec22.pdf).

For a stationary scalar field, choose the carrier convention $e^{-i2\pi\nu t}$, with [frequency](frequency.md) $\nu$ in cycles per second. Let $S(\nu)\geq0$ be its [spectral density](spectral-density-of-a-stationary-process.md) per unit [frequency](frequency.md), with $0<\int S(\nu)\,d\nu<\infty$. Its normalized field correlation is the [Fourier transform](fourier-transform.md)

$$
g^{(1)}(\tau)=\frac{\int S(\nu)e^{-i2\pi\nu\tau}\,d\nu}{\int S(\nu)\,d\nu}.
$$

The [optical spectrum](optical-spectrum.md) weights the rotating contributions; a broad spread of [frequencies](frequency.md) allows them to cancel at short delays. This is the stationary field correlation–spectrum relation. The relevant spectrum is that of the optical field in the detected mode, rather than the low-frequency fluctuations of a detector's [light intensity](light-intensity.md). [Rüdiger Paschotta, RP Photonics Encyclopedia, Optical Spectrum: optical field spectrum and temporal coherence](https://www.rp-photonics.com/optical_spectrum.html).

Here are two stipulated line profiles, each centered at $\nu_0$ with [full width at half maximum](full-width-at-half-maximum.md) $\Delta\nu>0$. Write $f=\nu-\nu_0$ and use normalized profiles on the whole detuning line:

$$
p_{\mathrm L}(f)=\frac{\Delta\nu/2}{\pi[f^2+(\Delta\nu/2)^2]},
\qquad p_{\mathrm G}(f)=\frac{2\sqrt{\ln2}}{\sqrt\pi\,\Delta\nu}\exp\!\left(-4\ln2\frac{f^2}{\Delta\nu^2}\right).
$$

The first is a Lorentzian, mathematically a [Cauchy distribution](cauchy-distribution.md); the second is a [Gaussian function](gaussian-function.md). Taking their [Fourier transforms](fourier-transform.md) gives, with the carrier factor $e^{-i2\pi\nu_0\tau}$ omitted from the magnitudes,

$$
|g^{(1)}_{\mathrm L}(\tau)|=e^{-\pi\Delta\nu|\tau|},
\qquad |g^{(1)}_{\mathrm G}(\tau)|=\exp\!\left(-\frac{\pi^2\Delta\nu^2\tau^2}{4\ln2}\right).
$$

These are calculated model results, not measured line profiles. The detuning approximation treats the narrow line as extending to arbitrarily large positive and negative $f$; for optical applications require $\Delta\nu\ll\nu_0$. Exact spectra of the complex positive-frequency field have no negative absolute [frequencies](frequency.md). Changing to [angular frequency](angular-frequency.md) replaces $\Delta\nu$ by $\Delta\omega/(2\pi)$; it must not silently preserve the same numerical constant.

<a id="image-michelson-interferometer-geometry-and-calculated-interferometric-visibility-versus-delay-for-stipulated-line-profiles"></a>
![](optical-coherence-delay-visibility.png)

**[Figure 27](#image-michelson-interferometer-geometry-and-calculated-interferometric-visibility-versus-delay-for-stipulated-line-profiles). Michelson interferometer geometry and calculated interferometric visibility versus delay for stipulated line profiles**.

Equal detected single-arm [light intensities](light-intensity.md) give [interferometric visibility](interferometric-visibility.md) equal to the correlation magnitude. Doubling the Gaussian [full width at half maximum](full-width-at-half-maximum.md) from $1$ to $2\,\mathrm{GHz}$ halves every fixed-contrast delay. At $\tau=0.5\,\mathrm{ns}$ the model gives Gaussian [interferometric visibility](interferometric-visibility.md) approximately $0.410686$ at $1\,\mathrm{GHz}$ and $0.0284471$ at $2\,\mathrm{GHz}$; the $1\,\mathrm{GHz}$ Lorentzian gives $0.207880$. The dashed curve instead keeps the $1\,\mathrm{GHz}$ Gaussian correlation and changes $I_2/I_1$ to $1/4$, multiplying all [interferometric visibilities](interferometric-visibility.md) by $0.8$. Its lower contrast at zero delay therefore comes entirely from intensity imbalance.

**Table of contents**

- [Optical coherence time](optical-coherence-time.md)
  - [Optical coherence length](optical-coherence-length.md)
- [Michelson interferometer](michelson-interferometer.md)

## ↑ Ancestors (7)

1. [First-order optical coherence](first-order-optical-coherence.md)
2. [Optical coherence](optical-coherence.md)
3. [Physical optics](physical-optics.md)
4. [Optics](optics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Optical coherence](optical-coherence.md)
- [Optical coherence time](optical-coherence-time.md)
- [Spatial optical coherence](spatial-optical-coherence.md)
- [Temporal optical coherence](temporal-optical-coherence.md)
