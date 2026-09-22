<h1 id="section-b/b2/spectrometer-and-resolution">Spectrometer and resolution</h1>

↑ **Parent:** [Solution](solution.md)

A non-polarizing [beam splitter](../../../../beam-splitter.md) divides the incident spectrum into a fixed arm and an arm with a translating mirror. Recombining their returned fields gives a detector signal as a function of mirror position $x$. The round-trip [optical path difference](../../../../optical-path-difference.md) is $D=2x$ relative to the equal-arm position, so the delay is $\tau=2x/c$ in air approximated as [vacuum](../../../../vacuum.md). Record both detector signal and calibrated position, subtract the constant background, and take a [Fourier transform](../../../../fourier-transform-split.md) of the [interferogram](../../../../interferogram.md).

<a id="section-b/b2/image-scanning-michelson-spectrometer-mirror-position-sets-delay-and-a-fourier-transform-of-the-recorded-interferogram-recovers-the-spectrum"></a>
![](../../../../past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2018-b2-fourier-spectrometer.png)

**[Figure 2](#section-b/b2/image-scanning-michelson-spectrometer-mirror-position-sets-delay-and-a-fourier-transform-of-the-recorded-interferogram-recovers-the-spectrum). Scanning Michelson spectrometer: mirror position sets delay, and a Fourier transform of the recorded interferogram recovers the spectrum**.

For matched arm polarizations and balanced throughput, write the ideal signal as

$$
I(\tau)=I_{\rm dc}+C\int_0^\infty S(\omega)\cos(\omega\tau)\,d\omega,
$$

where $S(\omega)$ is the incident spectral [power](../../../../power.md) density and $C$ is a constant set by the [beam splitter](../../../../beam-splitter.md) and detector. This is the cosine-transform form of [Fourier transform spectroscopy](../../../../fourier-transform-spectroscopy.md), or equivalently the [Wiener-Khinchin theorem](../../../../wiener-khinchin-theorem.md) applied to delayed self-interference.

The [delay-range resolution in Fourier transform spectroscopy](../../../../delay-range-resolution-in-fourier-transform-spectroscopy.md) follows because recording a finite delay range multiplies the correlation by a window. Its transform broadens each [spectral line](../../../../spectral-line.md) by an instrumental width of order the reciprocal delay range. A mirror travel range $L$ creates a delay range of order $2L/c$, so

$$
\delta\nu\sim\frac{c}{2L},\qquad
\delta\lambda\simeq\frac{\lambda^2}{c}\delta\nu,
\qquad \boxed{\delta\lambda\propto\frac{\lambda^2}{L}.}
$$

At fixed [wavelength](../../../../wavelength.md), absolute [wavelength](../../../../wavelength.md) resolution therefore improves inversely with travel range. The numerical coefficient depends on whether $L$ is a one-sided or total travel, on the window or apodization, and on whether resolution means first zero, half width or another criterion. The proportionality is the requested convention-independent result. Position sampling must also be fine enough to sample the fastest fringe variation without aliasing.

## ↑ Ancestors (14)

1. [Solution](solution.md)
2. [B2](../b2.md)
3. [Section B](../../section-b.md)
4. [2018](../../../2018-split.md)
5. [Past exam of the optics and electrodynamics course of the University of Cambridge](../../../split.md)
6. [Optics and Electrodynamics course of the University of Cambridge](../../../../optics-and-electrodynamics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../list-of-universities.md)
14. [Codex Wiki](../../../../split.md)
