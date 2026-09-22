<h1 id="section-b/b6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [transmission line](../../../../../../transmission-line.md) stores electric and magnetic [energy](../../../../../../energy-split.md) along its length, so [voltage](../../../../../../voltage.md) and current depend on both position and time. A distributed circuit uses [inductance](../../../../../../inductance.md) $L'$ and [capacitance](../../../../../../capacitance.md) $C'$ per length, together with resistance $R'$ and leakage conductance $G'$. Applying [voltage](../../../../../../voltage.md) and charge balance to a short segment gives the [telegrapher's equations](../../../../../../telegrapher-s-equations.md),

$$
\partial_xV=-R'I-L'\partial_tI,\qquad
\partial_xI=-G'V-C'\partial_tV.
$$

For a lossless line, both variables obey [wave equations](../../../../../../wave-equation-split.md) with speed $v=1/\sqrt{L'C'}$ and [characteristic impedance](../../../../../../characteristic-impedance.md) $Z_0=\sqrt{L'/C'}$. Forward and backward [waves](../../../../../../wave-split.md) obey $I^+=V^+/Z_0$ and $I^-=-V^-/Z_0$. Matching a termination $Z_L$ gives the [voltage](../../../../../../voltage.md) [reflection coefficient](../../../../../../reflection-coefficient.md)

$$
\boxed{\Gamma_L=\frac{Z_L-Z_0}{Z_L+Z_0}.}
$$

A matched load absorbs without reflection; an open circuit has $\Gamma_L=1$, and a short has $\Gamma_L=-1$. Reflections can produce [standing waves](../../../../../../standing-wave.md). A coaxial line confines the fields between conductors and, for a uniform [dielectric](../../../../../../dielectric.md) TEM [wave](../../../../../../wave-split.md), has $v=1/\sqrt{\mu\epsilon}$. Finite loss attenuates [waves](../../../../../../wave-split.md); frequency-dependent losses or material properties can also distort pulses. **A long line is a wave-carrying distributed system, so it cannot generally be replaced by one lumped capacitor.**

## ↑ Ancestors (15)

1. [A](../a.md)
2. [B6](../../b6.md)
3. [Section B](../../../section-b.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2012](../../../../split.md)
6. [Past exam of the physics B course of the University of Cambridge](../../../../../split.md)
7. [Physics B course of the University of Cambridge](../../../../../../physics-b-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
