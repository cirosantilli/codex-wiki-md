<h1 id="section-b/b2/equally-spaced-spectral-components">Equally spaced spectral components</h1>

↑ **Parent:** [Solution](solution.md)

For $N$ equal-intensity lines of spacing $\Delta\omega$, sum their correlations as a [geometric series](../../../../geometric-series.md):

$$
\sum_{n=0}^{N-1}e^{-i(\omega_0+n\Delta\omega)\tau}
=e^{-i[\omega_0+(N-1)\Delta\omega/2]\tau}
\frac{\sin(N\Delta\omega\tau/2)}{\sin(\Delta\omega\tau/2)}.
$$

The [interferogram of an equally spaced spectral multiplet](../../../../interferogram-of-an-equally-spaced-spectral-multiplet.md) has normalized visibility

$$
\mathcal V_N(\tau)=\left|\frac{\sin(N\Delta\omega\tau/2)}{N\sin(\Delta\omega\tau/2)}\right|.
$$

In the second original plot, full revivals occur at approximately $\tau=0,\pm100,\pm200\,\mathrm{ps}$, so

$$
\boxed{\Delta\omega=\frac{2\pi}{100\,\mathrm{ps}}\simeq6.28\times10^{10}\,\mathrm{rad\,s^{-1}},\qquad\Delta\nu\simeq10.0\,\mathrm{GHz}.}
$$

Between $0$ and $100\,\mathrm{ps}$ there are three zeros, near $25$, $50$ and $75\,\mathrm{ps}$, and two small subsidiary lobes. Since the model has $N-1$ zeros between adjacent revivals,

$$
\boxed{N=4.}
$$

The peak envelope of about $8$ and the intensity background of about $8$ are consistent with four equal components in the source's normalization, but the internal zero count is the useful shape-based check. The inference assumes the equal spectral weights represented by the graph; revival spacing alone does not fix the number of lines, and arbitrary unequal or hidden components would require more spectral information. Delayed self-interference measures spectral powers, not the relative phases between different source frequencies, so these revivals alone do not prove that the source emits a phase-locked pulse train.

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
