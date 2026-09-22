<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The real [odd function](../../../../../odd-function.md) has a purely imaginary odd [Fourier transform](../../../../../fourier-transform-split.md). Setting $A=\pi/2$ and using a product-to-sum identity,

$$
\begin{aligned}
\widetilde f(k)&=-2i\int_0^A\sin x\sin(kx)\,dx\\
&=-i\left[\frac{\sin[(k-1)A]}{k-1}-\frac{\sin[(k+1)A]}{k+1}\right]\\
&=\boxed{\frac{2ik\cos(\pi k/2)}{k^2-1}},\qquad k\ne\pm1.
\end{aligned}
$$

The apparent singularities are removable. Direct evaluation or limits give

$$
\boxed{\widetilde f(1)=-\frac{i\pi}{2},\qquad\widetilde f(-1)=\frac{i\pi}{2},\qquad\widetilde f(0)=0.}
$$

In particular, the transform stays finite where its numerator and denominator both vanish.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
