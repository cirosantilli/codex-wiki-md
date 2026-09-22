<h1 id="5/a/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Multiply $H$ by the exponential form of the sine and use the [modulation property of the Fourier transform](../../../../../../modulation-property-of-the-fourier-transform.md):

$$
\widetilde f(\omega)=\frac1{2i}[\widetilde H(\omega-\omega_0)-\widetilde H(\omega+\omega_0)].
$$

Inserting part (iii) gives

$$
\boxed{\widetilde f(\omega)=\frac12\left[\operatorname{PV}\frac1{\omega+\omega_0}-\operatorname{PV}\frac1{\omega-\omega_0}\right]+\frac\pi{2i}[\delta(\omega-\omega_0)-\delta(\omega+\omega_0)].}
$$

The reciprocal terms are real principal-value distributions and the delta terms are imaginary. Equivalently, exponential damping $H(t)e^{-\epsilon t}$ gives $\omega_0/[(\epsilon+i\omega)^2+\omega_0^2]$, whose distributional limit is the boxed expression. The shifted-difference formula remains valid at $\omega_0=0$, where all terms cancel.

## ↑ Ancestors (14)

1. [Iv](../iv.md)
2. [A](../../a.md)
3. [5](../../../5.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
