# Nuclear resonance linewidth

↑ **Parent:** [Continuous-wave nuclear magnetic resonance](continuous-wave-nuclear-magnetic-resonance.md)

For weak drive in this homogeneous model, half maximum occurs at $|\Delta|=1/T_2$. The absorption [full width at half maximum](full-width-at-half-maximum.md) is therefore

$$
\Delta\omega_{\rm FWHM}=\frac2{T_2},\qquad
\Delta f_{\rm FWHM}=\frac1{\pi T_2},\qquad
\Delta B_{\rm FWHM}=\frac2{|\gamma|T_2}.
$$

The example gives $2.653\,\mathrm{Hz}$ or $0.06230\,\mathrm{\mu T}$. At finite drive the model width is multiplied by $\sqrt{1+s}$. Field inhomogeneity and unresolved components can also broaden an actual line, so its width alone does not determine pure [dephasing](dephasing-channel.md).

The same width appears by an original [Fourier transform](fourier-transform-split.md) calculation. For $a=1/T_2$ and a free homogeneous [signal](signal.md) demodulated exactly at resonance,

$$
\int_0^\infty e^{-at}e^{i\Omega t}\,dt=\frac1{a-i\Omega},\qquad
\operatorname{Re}\frac1{a-i\Omega}=\frac{a}{a^2+\Omega^2}.
$$

This connects exponential memory to a Lorentzian absorptive line. It is a mathematical connection, not evidence that the 1946 teams performed pulsed [Fourier transform](fourier-transform-split.md) spectroscopy. Instrumental [signal bandwidth](signal-bandwidth.md) is a separate choice: narrowing a receiver band can reject [thermal electrical noise](thermal-electrical-noise.md), but too narrow a band distorts a changing [signal](signal.md). A sample linewidth and a receiver bandwidth are not interchangeable.

## ↑ Ancestors (4)

1. [Continuous-wave nuclear magnetic resonance](continuous-wave-nuclear-magnetic-resonance.md)
2. [Nuclear magnetic resonance](nuclear-magnetic-resonance-split.md)
3. [Chemistry](chemistry-split.md)
4. [Codex Wiki](split.md)
