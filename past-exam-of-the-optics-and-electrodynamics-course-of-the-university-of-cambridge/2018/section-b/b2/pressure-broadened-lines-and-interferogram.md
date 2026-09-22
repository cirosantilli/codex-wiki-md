<h1 id="section-b/b2/pressure-broadened-lines-and-interferogram">Pressure-broadened lines and interferogram</h1>

↑ **Parent:** [Solution](solution.md)

Interpret the stated $\tau_1=1\,\mathrm{ns}$ as the coherence-decay time, or the mean interval between fully phase-randomizing collisions in the simple impact model of [pressure broadening](../../../../pressure-broadening.md). Then each line has correlation $e^{-|\tau|/\tau_1}e^{-i\omega_j\tau}$. The [collisional phase relaxation and Lorentzian linewidth](../../../../collisional-phase-relaxation-and-lorentzian-linewidth.md) transform gives

$$
L_j(\omega)=\frac1\pi\frac{1/\tau_1}{(\omega-\omega_j)^2+(1/\tau_1)^2},
\qquad \boxed{\Delta\omega_{\rm FWHM}=\frac2{\tau_1}=2.0\times10^9\,\mathrm{rad\,s^{-1}},\quad
\Delta\nu_{\rm FWHM}=\frac1{\pi\tau_1}=0.318\,\mathrm{GHz}.}
$$

The intrinsic spectrum is the sum of two such [Lorentzian line shapes](../../../../lorentzian-line-shape.md), still centred $5.0\,\mathrm{GHz}$ apart. With equal weights and balanced arms, its normalized visibility is

$$
\boxed{\mathcal V(\tau)=e^{-|\tau|/\tau_1}|\cos(\Delta\omega\tau/2)|.}
$$

For the intensity normalization of the first source plot, the corresponding model [interferogram](../../../../interferogram.md) is

$$
I(\tau)=4+4e^{-|\tau|/\tau_1}\cos(\Delta\omega\tau/2)\cos(\bar\omega\tau).
$$

The constant background remains $4$; only the oscillatory contrast decays. The beating zeros and recurrence spacing remain fixed, but successive visibility revivals shrink, reaching a factor $e^{-0.2}\simeq0.819$ at $|\tau|=200\,\mathrm{ps}$ and $e^{-1}$ at $1\,\mathrm{ns}$. Long-delay fringes disappear toward the background.

<a id="section-b/b2/image-calculated-pressure-broadened-interferogram-decaying-visibility-revivals-and-lorentzian-doublet-for-a-one-nanosecond-coherence-time"></a>
![](../../../../past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2018-b2-pressure-broadening.png)

**[Figure 3](#section-b/b2/image-calculated-pressure-broadened-interferogram-decaying-visibility-revivals-and-lorentzian-doublet-for-a-one-nanosecond-coherence-time). Calculated pressure-broadened interferogram, decaying visibility revivals and Lorentzian doublet for a one-nanosecond coherence time**.

The sketch chooses a carrier [frequency](../../../../frequency.md) for legibility; the envelope and linewidth follow from the inferred spacing and specified coherence time. A finite experimental delay window additionally convolves these intrinsic Lorentzians with the instrumental line profile. If $\tau_1$ were instead a population lifetime, the lifetime-limited field decay rate would be $1/(2\tau_1)$ and the corresponding linewidth would be half the boxed value. The source does not define that time convention explicitly; pressure-collision coherence decay is the interpretation used here.

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
