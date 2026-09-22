<h1 id="section-b/b8/solution">Solution</h1>

↑ **Parent:** [B8](../b8.md)

**Packet and group index.** A [wave packet](../../../../../wave-packet.md) superposes nearby [wavevectors](../../../../../wavevector.md) to form a localized envelope. The [phase velocity](../../../../../phase-velocity.md) is $v_p=\omega/k$; for a narrow packet with weak distortion the envelope velocity is $v_g=d\omega/dk$. Since $k=2\pi fn(f)/c$,

$$
\boxed{\frac c{v_g}=n_g=n+f\frac{dn}{df}}.
$$

For the stipulated linear index, $n_g=1.5+\tau(2f-f_0)$, not simply $n(f)$.

**[bandwidth](../../../../../bandwidth-signal-processing.md) and speed spread.** A pulse lasting $t_p$ has Fourier [bandwidth](../../../../../bandwidth-signal-processing.md) of order $1/t_p$, so $\Delta f\sim10^{10}\ \mathrm{Hz}$; an exact width coefficient depends on pulse shape and width convention. At the carrier,

$$
\boxed{n_g(f_0)=1.56,\qquad v_g(f_0)=\frac c{1.56}\simeq1.92\times10^8\ \mathrm{m\,s^{-1}}}.
$$

Across a full [bandwidth](../../../../../bandwidth-signal-processing.md) $\Delta f$,

$$
\Delta n_g=2\tau\Delta f=6.0\times10^{-6},\qquad
\boxed{\Delta v_g\simeq\frac{2c\tau\Delta f}{1.56^2}\simeq7.4\times10^2\ \mathrm{m\,s^{-1}}}.
$$

Higher-frequency components have the lower [group velocity](../../../../../group-velocity.md). For a band symmetric about $f_0$, the endpoint velocities are approximately $v_g(f_0)\pm370\ \mathrm{m\,s^{-1}}$.

**[dispersion-limited digital-fibre link length](../../../../../dispersion-limited-digital-fibre-link-length.md).** Differential [group delay](../../../../../group-delay.md) accumulates as

$$
\Delta t_{\rm disp}=L\Delta(1/v_g)=\frac{2\tau L\Delta f}{c}
\simeq(2.0\times10^{-14}\ \mathrm{s\,m^{-1}})L.
$$

The pulse spacing is $t_r=10^{-9}\ \mathrm s$. Pulse overlap and intersymbol interference become serious when the dispersive spread approaches that spacing, giving

$$
\boxed{L_{\max}\sim\frac{ct_r}{2\tau\Delta f}\simeq50\ \mathrm{km}}.
$$

A conservative full-width estimate $t_p+\Delta t_{\rm disp}\lesssim t_r$ gives about **45 km**; this refinement is not a universal sharp boundary because pulse shape, chirp and detection tolerance are unspecified. Attenuation and modal or waveguide dispersion could impose further limits, but are not quantified by the supplied index law.

**[digital optical pulse regeneration](../../../../../digital-optical-pulse-regeneration.md).** Each stage must recover and regenerate the data with fresh, short pulses and correct timing, as well as restore signal level. Amplifying the already broadened waveform alone does not remove accumulated dispersion; explicit dispersion compensation is an alternative to full regeneration.

## ↑ Ancestors (14)

1. [B8](../b8.md)
2. [Section B](../../section-b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2013](../../../split.md)
5. [Past exam of the physics A course of the University of Cambridge](../../../../split.md)
6. [Physics A course of the University of Cambridge](../../../../../physics-a-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
