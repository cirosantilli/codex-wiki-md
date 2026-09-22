# Optical coherence time

↑ **Parent:** [Temporal optical coherence](temporal-optical-coherence.md)

An [optical coherence time](optical-coherence-time.md) summarizes the delay scale of [temporal optical coherence](temporal-optical-coherence.md), but requires a convention. Two useful choices are the first positive delay $\tau_{1/e}$ where $|g^{(1)}|=e^{-1}$, for a monotonically decaying envelope, and the integral definition

$$
\tau_{\mathrm{int}}=\int_{-\infty}^{\infty}|g^{(1)}(\tau)|^2\,d\tau.
$$

The latter counts correlation over both signs of delay and may diverge for ideal discrete lines. [Paschotta, Coherence Time: exponential time constant and integral definition](https://www.rp-photonics.com/coherence_time.html).

For the stipulated Lorentzian and Gaussian profiles in [temporal optical coherence](temporal-optical-coherence.md), direct substitution and a [Gaussian integral](gaussian-integral.md) give

$$
\begin{array}{c|cc}
\text{profile}&\tau_{1/e}&\tau_{\mathrm{int}}\\
\hline
\text{Lorentzian}&1/(\pi\Delta\nu)&1/(\pi\Delta\nu)\\
\text{Gaussian}&2\sqrt{\ln2}/(\pi\Delta\nu)&\sqrt{2\ln2/\pi}/\Delta\nu
\end{array}
$$

The respective dimensionless coefficients are $0.318310$ for both Lorentzian conventions, and $0.530021$ and $0.664282$ for the Gaussian conventions. The familiar scale $1/\Delta\nu$ is consequently an estimate, not a convention-independent equality. A source with narrow discrete lines can have repeated revivals instead of one monotonically decaying envelope, so recording the full $|g^{(1)}(\tau)|$ can be more informative than one [optical coherence time](optical-coherence-time.md).

**Table of contents**

- [Optical coherence length](optical-coherence-length.md)
  - [Coherence length from a finite spectral band](coherence-length-from-a-finite-spectral-band.md)

## ↑ Ancestors (8)

1. [Temporal optical coherence](temporal-optical-coherence.md)
2. [First-order optical coherence](first-order-optical-coherence.md)
3. [Optical coherence](optical-coherence.md)
4. [Physical optics](physical-optics-split.md)
5. [Optics](optics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (10)

- [Coherence length from a finite spectral band](coherence-length-from-a-finite-spectral-band.md)
- [Finite-response stellar intensity correlations](finite-response-stellar-intensity-correlations.md)
- [Homogeneous spectral broadening](homogeneous-spectral-broadening.md)
- [Lifetime broadening](lifetime-broadening.md)
- [Optical coherence length](optical-coherence-length.md)
- [Optical coherence time](optical-coherence-time.md)
- [Optical path delay in crossed-beam interference](optical-path-delay-in-crossed-beam-interference.md)
- [Optical path length](optical-path-length.md)
- [Solution](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2015/paper-1/2/b/solution.md)
- [Longitudinal coherence estimate](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2019/section-a/a3/longitudinal-coherence-estimate.md)
