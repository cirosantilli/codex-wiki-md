<h1 id="section-a/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [Johnson-Nyquist noise](../../../../thermal-electrical-noise.md) formula gives the open-circuit mean-square [voltage](../../../../voltage.md) in a small [frequency](../../../../frequency.md) band $d\nu$. When a source [electrical resistance](../../../../electrical-resistance.md) $R$ drives a load $R$ with [impedance matching](../../../../impedance-matching.md), the load sees half the source [voltage](../../../../voltage.md), so the available noise [power](../../../../power.md) is

$$
dP_t=\frac{\langle V^2\rangle/4}{R}=k_BT_t\,d\nu.
$$

The factor of four in the open-circuit formula is therefore not an extra factor in the delivered [power](../../../../power.md).

The transmitter's [antenna gain](../../../../antenna-gain.md) $G$ makes the axial spectral [energy flux](../../../../energy-flux.md) at range $d$

$$
\frac{dS}{d\nu}=\frac{G}{4\pi d^2}k_BT_t.
$$

Multiplication by the receiving [antenna effective area](../../../../antenna-effective-area.md) $A$ gives $dP_r=k_BT_tGA\,d\nu/(4\pi d^2)$. Define the equivalent receiving [antenna temperature](../../../../antenna-temperature.md) $T_A$ by the available matched-load noise $dP_r=k_BT_A\,d\nu$. Then

$$
\boxed{T_A=T_t\frac{GA}{4\pi d^2}
=(10^4\,\mathrm K)\frac{10^5(1.8\,\mathrm{m^2})}{4\pi(10^3\,\mathrm m)^2}
=143.24\,\mathrm K\simeq143\,\mathrm K.}
$$

This is the transmitter-induced equivalent [noise temperature](../../../../noise-temperature.md) of the receiver port. It does not determine the actual physical [temperature](../../../../temperature-split.md) of its internal [electrical resistance](../../../../electrical-resistance.md), or any additional receiver and background noise. The calculation assumes the usual far-field link, negligible path loss beyond geometric spreading, matched [polarization of an electromagnetic wave](../../../../polarization-of-an-electromagnetic-wave.md) at the two antennas and the stated effective collecting area. No additional one-half polarization factor is needed for the matched polarization of radiation from one transmitting [antenna](../../../../antenna-radio.md).

## ↑ Ancestors (13)

1. [2](../2.md)
2. [Section A](../../section-a.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the optics and electrodynamics course of the University of Cambridge](../../../split.md)
5. [Optics and Electrodynamics course of the University of Cambridge](../../../../optics-and-electrodynamics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
