<h1 id="section-b/b3/returned-pulse-power">Returned pulse power</h1>

↑ **Parent:** [Solution](solution.md)

The receiving dipole remains matched. To model its actual reradiation, let its feed impedance be $R_{\rm rad}+iX$ with no ohmic loss, and its matched load be $R_{\rm rad}-iX$. The induced current dissipates equal powers in the load and in [radiation resistance](../../../../radiation-resistance.md). Thus [matched-load scattering of a Hertzian dipole](../../../../matched-load-scattering-of-a-hertzian-dipole.md) has $P_{\rm sca}=P_2$, even though its port is matched.

The scattered wave has the same dipole gain toward the original antenna. Applying the reciprocal link factor a second time gives the [reciprocal Hertzian-dipole echo](../../../../reciprocal-hertzian-dipole-echo.md):

$$
\eta=G_tG_r\left(\frac{\lambda}{4\pi r}\right)^2\simeq1.28\times10^{-5},\qquad
\boxed{P_{\rm echo}=P_0\eta^2\simeq1.64\times10^{-10}\,\mathrm W=0.164\,\mathrm{nW},\quad P_{\rm echo}\propto r^{-4}.}
$$

Each leg supplies an inverse-square spreading factor. This is the carrier-averaged [power](../../../../power.md) during a returned pulse with the stated transmitted [power](../../../../power.md) during its pulse. The pulse-train average additionally depends on duty cycle, which is not given. Treating the pulses as narrowband keeps the same gain and [wavelength](../../../../wavelength.md) approximation.

A matched feed does not make a physical dipole a perfect absorber with zero external scattering. A model retaining only an [antenna load-mismatch echo](../../../../antenna-load-mismatch-echo.md) would set its reflected travelling-port wave to zero and would not determine this reradiation. Conversely, an arbitrary antenna structure can add scattering not fixed by gain and effective area alone. The numerical answer uses the ideal lossless Hertzian-dipole scattering model just stated.

## ↑ Ancestors (14)

1. [Solution](solution.md)
2. [B3](../b3.md)
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
