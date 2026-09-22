<h1 id="section-b/8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The original diagram has a [series circuit](../../../../../series-circuit.md) containing $R$ and $L$, in parallel with $C$; it is not three separate parallel components. The [electrical admittance](../../../../../electrical-admittance.md) is therefore

$$
Y=\frac1Z=\frac1{R+i\omega L}+i\omega C=\frac R{R^2+\omega^2L^2}+i\left[\omega C-\frac{\omega L}{R^2+\omega^2L^2}\right].
$$

For $R>0$, voltage and current are in phase when the [imaginary part](../../../../../imaginary-part.md) of $Y$ vanishes. Excluding the zero-[frequency](../../../../../frequency.md) solution, division by $\omega$ gives

$$
C=\frac L{R^2+\omega_r^2L^2},\qquad\boxed{\omega_r=\sqrt{\frac1{LC}-\frac{R^2}{L^2}}.}
$$

A nonzero [lossy parallel coil resonance](../../../../../lossy-parallel-coil-resonance.md) exists only if $L>R^2C$. With $R=10\,\Omega$, $L=0.150\,\mathrm H$ and $C=1.00\times10^{-5}\,\mathrm F$,

$$
\omega_r=\sqrt{666666.7-4444.44}\,\mathrm{s^{-1}}=\boxed{813.77\,\mathrm{rad\,s^{-1}}},\qquad\boxed{f_r=\frac{\omega_r}{2\pi}=129.52\,\mathrm{Hz}.}
$$

For zero [electrical resistance](../../../../../electrical-resistance.md), the ideal parallel [inductor](../../../../../inductor.md)-[capacitor](../../../../../capacitor.md) cancellation occurs at

$$
\boxed{\omega_0=\frac1{\sqrt{LC}}=816.50\,\mathrm{rad\,s^{-1}},\qquad f_0=129.95\,\mathrm{Hz}.}
$$

The fractional reduction relative to the zero-resistance coil is

$$
\boxed{\frac{f_0-f_r}{f_0}=1-\sqrt{1-\frac{R^2C}{L}}=0.00333891=0.3339\%.}
$$

At exactly $R=0$ and $\omega=\omega_0$, $Y=0$, so finite applied voltage draws zero net current in the ideal model. The quoted [frequency](../../../../../frequency.md) is the limiting parallel-resonance value; the phase of an exactly zero current is undefined.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [8](../../8.md)
3. [Section B](../../../section-b.md)
4. [2022](../../../../2022-split.md)
5. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
