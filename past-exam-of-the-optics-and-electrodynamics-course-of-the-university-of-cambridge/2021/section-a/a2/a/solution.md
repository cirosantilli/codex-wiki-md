<h1 id="section-a/a2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The transmitting [antenna](../../../../../antenna-radio.md) is matched to its input [transmission line](../../../../../transmission-line.md), so its real terminal [electrical resistance](../../../../../electrical-resistance.md) is $Z_i$. The identical receiving [antenna](../../../../../antenna-radio.md) has the same [electrical impedance](../../../../../electrical-impedance.md) at the operating [frequency](../../../../../frequency.md). Its available received [power](../../../../../power.md) for a matched load is the incident [energy flux](../../../../../energy-flux.md) times its [antenna effective area](../../../../../antenna-effective-area.md):

$$
P_{\rm av}=\frac{P_iG_a}{4\pi d^2}A_e
=P_i\left(\frac{G_a\lambda}{4\pi d}\right)^2\equiv P_i\mathcal F.
$$

The real receiving load is $Z_t$, so its voltage-wave [reflection coefficient](../../../../../reflection-coefficient.md) relative to $Z_i$ is $\Gamma_L=(Z_t-Z_i)/(Z_t+Z_i)$. The fraction of available [power](../../../../../power.md) delivered to the output line is

$$
1-|\Gamma_L|^2=\frac{4Z_iZ_t}{(Z_i+Z_t)^2}.
$$

Consequently, neglecting path losses, mismatch of [polarization of an electromagnetic wave](../../../../../polarization-of-an-electromagnetic-wave.md) and line losses,

$$
\boxed{P_t=P_i\left(\frac{G_a\lambda}{4\pi d}\right)^2
\frac{4Z_iZ_t}{(Z_i+Z_t)^2}.}
$$

This is the [Friis transmission equation](../../../../../friis-transmission-equation.md) with a receiving impedance-mismatch factor. For fixed $P_i,G_a,d,Z_i,Z_t$, it scales as $\lambda^2$. That scaling is conditional on holding [antenna gain](../../../../../antenna-gain.md) fixed: a fixed physical aperture can instead have $G_a\propto\lambda^{-2}$, and any [wavelength](../../../../../wavelength.md) dependence of the impedances also enters the expression. The matched-output check $Z_t=Z_i$ gives $P_t=P_i\mathcal F$.

## ↑ Ancestors (14)

1. [A](../a.md)
2. [A2](../../a2.md)
3. [Section A](../../../section-a.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the optics and electrodynamics course of the University of Cambridge](../../../../split.md)
6. [Optics and Electrodynamics course of the University of Cambridge](../../../../../optics-and-electrodynamics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
