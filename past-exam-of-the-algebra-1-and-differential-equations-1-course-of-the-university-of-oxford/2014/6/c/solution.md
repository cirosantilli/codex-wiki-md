<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Complete the square inside the [Fourier transform](../../../../fourier-transform-split.md) of the [Gaussian heat kernel](../../../../gaussian-heat-kernel.md):

$$
-\frac{x^2}{4t}-i\omega x
=-\left(\frac{x}{2\sqrt t}+i\sqrt t\,\omega\right)^2-t\omega^2.
$$

After $z=x/(2\sqrt t)$,

$$
\widehat q_t(\omega)=\frac{e^{-t\omega^2}}{\sqrt\pi}
\int_{-\infty}^{\infty}e^{-(z+i\sqrt t\,\omega)^2}\,dz.
$$

The supplied shifted [Gaussian integral](../../../../gaussian-integral.md) equals $\sqrt\pi$ for real $\sqrt t\,\omega$. Hence

$$
\boxed{\widehat q_t(\omega)=e^{-t\omega^2}.}
$$

At zero this says $\int q_t=1$, so convolution with the heat kernel averages rather than rescales the initial mass. The formula is an instance of the [Fourier transform of a Gaussian](../../../../fourier-transform-of-a-gaussian.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [6](../../6.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the algebra 1 and differential equations 1 course of the University of Oxford](../../../split.md)
5. [Algebra 1 and differential equations 1 course of the University of Oxford](../../../../algebra-1-and-differential-equations-1-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
