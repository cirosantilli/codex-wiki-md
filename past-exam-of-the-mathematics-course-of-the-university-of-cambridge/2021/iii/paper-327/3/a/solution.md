<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $\omega\ne0$, insert the Gaussian damping factor $e^{-\varepsilon x^2/2}$ and use the [Gaussian integral](../../../../../../gaussian-integral.md):

$$
\int_{\mathbb R}
e^{-(\varepsilon-i\omega)x^2/2-i\lambda x}\,dx
=\sqrt{\frac{2\pi}{\varepsilon-i\omega}}
\exp\left[-\frac{\lambda^2}{2(\varepsilon-i\omega)}\right].
$$

Taking $\varepsilon\downarrow0$ in $\mathcal S'$ with the continuous square-root branch gives the [Fresnel integral](../../../../../../fresnel-integral.md)

$$
\boxed{
\mathcal F\left[e^{i\omega x^2/2}\right](\lambda)
=\sqrt{\frac{2\pi}{|\omega|}}
e^{i\pi\operatorname{sgn}(\omega)/4}
e^{-i\lambda^2/(2\omega)}}.
$$

For $\omega=0$, the function is constant and its Fourier transform is $\boxed{2\pi\delta_0}$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 327](../../../paper-327-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
