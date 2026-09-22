<h1 id="2/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the [Fourier transform](../../../../../fourier-transform-split.md) convention $\widehat W(k,z,t)=\int_{\mathbb R}W(x,z,t)e^{-ikx}dx$, with inverse factor $1/(2\pi)$. The initial profile occupies only the vertical mode $\sin(\pi z/h)$. Its transform is

$$
\widehat W(k,z,0)=\pi hC e^{-\epsilon h|k|}\sin(\pi z/h),\qquad \widehat W_t(k,z,0)=0.
$$

The transformed evolution is a [harmonic oscillator](../../../../../simple-harmonic-motion.md) for each $k$, with

$$
\omega(k)=\frac{\sqrt{\alpha g}\,k}{\sqrt{k^2+\pi^2/h^2+\alpha^2/4}}.
$$

Therefore inversion gives

$$
\boxed{W(x,z,t)=\frac{hC}{2}\sin\!\left(\frac{\pi z}{h}\right)\int_{-\infty}^{\infty}e^{-\epsilon h|k|}\cos(\omega(k)t)e^{ikx}\,dk}.
$$

Using the nonnegative even frequency instead gives the same cosine. At $t=0$, $\int_{\mathbb R}e^{-a|k|}e^{ikx}dk=2a/(a^2+x^2)$ with $a=\epsilon h$, recovering the specified initial profile and its zero time derivative.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the waves and compressible flow course of the University of Oxford](../../../../split.md)
6. [Waves and compressible flow course of the University of Oxford](../../../../../waves-and-compressible-flow-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
