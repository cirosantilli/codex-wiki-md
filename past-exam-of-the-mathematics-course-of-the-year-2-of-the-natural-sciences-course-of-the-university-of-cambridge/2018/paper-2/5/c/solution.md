<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\beta=\sqrt{\Omega^2-\kappa^2}$, interpreted as $i\sqrt{\kappa^2-\Omega^2}$ in the [overdamped](../../../../../overdamping.md) case. Factoring the denominator gives

$$
\Omega^2-\omega^2+2i\kappa\omega=-(\omega-\omega_-)(\omega-\omega_+),\qquad
\boxed{\omega_\pm=i\kappa\pm\beta}.
$$

[Fourier inversion](../../../../../fourier-inversion-theorem.md) and the [convolution theorem](../../../../../convolution-theorem.md) give

$$
\boxed{y(t)=\int_{-\infty}^{\infty}G(t-\xi)f(\xi)\,d\xi},
$$

where

$$
G(t)=-\frac1{2\pi}\int_{-\infty}^{\infty}
\frac{e^{i\omega t}}{(\omega-\omega_-)(\omega-\omega_+)}\,d\omega.
$$

Thus the requested numerator is

$$
\boxed{s(\omega,t)=-\frac1{2\pi}e^{i\omega t}}.
$$

For all positive $\kappa,\Omega$, both [poles](../../../../../pole.md) lie in the upper half-plane. In the [overdamped](../../../../../overdamping.md) case their imaginary parts are $\kappa\pm\sqrt{\kappa^2-\Omega^2}$, both positive. At equality they merge into a double [pole](../../../../../pole.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
