<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

At $\Omega=3/4$, the two continuous triangles overlap near zero. Their amplitudes add, giving a central plateau. Explicitly, write $C(\omega)$ for the continuous part of $\widetilde\phi$:

$$
C(\omega)=\begin{cases}\pi/4,&|\omega|\leq1/4,\\\dfrac\pi2(1/4+|\omega|),&1/4<|\omega|\leq3/4,\\\dfrac\pi2(7/4-|\omega|),&3/4<|\omega|<7/4,\\0,&|\omega|\geq7/4.\end{cases}
$$

There are also the two carrier [Dirac delta](../../../../../dirac-delta-function.md) lines $\pi\delta(\omega\mp3/4)$. The last panel of the preceding figure shows this spectrum and the retained central portion. The prescribed strict cutoff removes the carriers and keeps

$$
\boxed{\widetilde\rho(\omega)=\begin{cases}\pi/4,&|\omega|\leq1/4,\\\dfrac\pi2(1/4+|\omega|),&1/4<|\omega|<3/4,\\0,&|\omega|\geq3/4.\end{cases}}
$$

The values of the ordinary function at individual endpoints do not affect its inverse transform. To handle the carrier lines, one must additionally assign zero filter gain to those lines, as the carrier-rejecting prescription indicates. A discontinuous mask has no canonical product with a [Dirac delta](../../../../../dirac-delta-function.md) at its discontinuity; a different physical boundary gain would leave a corresponding multiple of $\cos(3t/4)$.

The retained spectrum is real and even. Its inverse [Fourier transform](../../../../../fourier-transform-split.md) is

$$
\rho(t)=\frac14\int_0^{1/4}\cos(\omega t)\,d\omega+\frac12\int_{1/4}^{3/4}(1/4+\omega)\cos(\omega t)\,d\omega.
$$

Integrating the linear factors yields

$$
\boxed{\rho(t)=\frac{\sin(3t/4)}{2t}+\frac{\cos(3t/4)-\cos(t/4)}{2t^2},\qquad t\neq0.}
$$

The removable value is $\boxed{\rho(0)=1/4}$, obtained either by expansion or by integrating $\widetilde\rho/(2\pi)$. Because the carrier [frequency](../../../../../frequency.md) is below the message bandwidth, this is [Fourier filtering of overlapping amplitude-modulation sidebands](../../../../../fourier-filtering-of-overlapping-amplitude-modulation-sidebands.md); the usual picture of two isolated bands in [single-sideband modulation](../../../../../single-sideband-modulation.md) does not apply without that qualification.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
