<h1 id="section-b/b6/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Put $\delta=k_Ml$. Eliminating the middle-segment [complex amplitudes](../../../../../../complex-amplitude.md) using the right-hand [boundary conditions](../../../../../../boundary-condition.md) gives

$$
1+r=t\left(\cos\delta-i\frac{Z_R}{Z_M}\sin\delta\right),\qquad
Z_L(1-r)=t\left(Z_R\cos\delta-iZ_M\sin\delta\right).
$$

Hence the displacement [reflection coefficient](../../../../../../reflection-coefficient.md) is

$$
r=\frac{(Z_L-Z_R)\cos\delta+i(Z_M-Z_LZ_R/Z_M)\sin\delta}
{(Z_L+Z_R)\cos\delta-i(Z_M+Z_LZ_R/Z_M)\sin\delta}.
$$

For finite positive real [mechanical impedances](../../../../../../mechanical-impedance.md), its denominator cannot vanish at real $\delta$. The real and imaginary parts of the numerator must therefore vanish separately:

$$
(Z_L-Z_R)\cos\delta=0,\qquad (Z_M^2-Z_LZ_R)\sin\delta=0.
$$

This gives all three possibilities.

If the exterior strings differ, $Z_L\ne Z_R$, then $\cos\delta=0$, so $\sin\delta\ne0$ and

$$
\boxed{Z_M=\sqrt{Z_LZ_R},\qquad l=\frac{(2n+1)\lambda_M}{4},\quad n=0,1,2,\ldots.}
$$

The middle segment is a [quarter-wave impedance transformer](../../../../../../quarter-wave-impedance-transformer.md). Its two reflected contributions cancel at these odd quarter-[wavelength](../../../../../../wavelength.md) thicknesses. Here $\lambda_M=2\pi/k_M$ is specifically the [wavelength](../../../../../../wavelength.md) in the middle string; the matching is not generally valid at every [frequency](../../../../../../frequency.md).

If $Z_L=Z_R$ but $Z_M$ differs, the second condition requires $\sin\delta=0$, giving

$$
\boxed{l=\frac{n\lambda_M}{2},\quad n=1,2,\ldots.}
$$

A whole number of half-[wavelengths](../../../../../../wavelength.md) reproduces the exterior [mechanical impedance](../../../../../../mechanical-impedance.md) at the input. The formal $n=0$ limit is zero [frequency](../../../../../../frequency.md) or zero segment length, rather than a finite-[wavelength](../../../../../../wavelength.md) resonance.

Finally, if $Z_L=Z_M=Z_R$, both conditions hold identically: $\boxed{r=0\text{ at every wavelength}}$. Since the system is lossless, each of these cases also gives unit transmitted [power](../../../../../../power.md).

## ↑ Ancestors (15)

1. [E](../e.md)
2. [B6](../../b6.md)
3. [Section B](../../../section-b.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the physics A course of the University of Cambridge](../../../../../split.md)
7. [Physics A course of the University of Cambridge](../../../../../../physics-a-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
