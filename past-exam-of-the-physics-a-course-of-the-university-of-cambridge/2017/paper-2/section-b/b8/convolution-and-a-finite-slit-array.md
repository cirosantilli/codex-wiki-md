<h1 id="section-b/b8/convolution-and-a-finite-slit-array">Convolution and a finite slit array</h1>

↑ **Parent:** [Solution](solution.md)

Use [Fourier transform](../../../../../fourier-transform-split.md) convention $\widehat f(q)=\int f(x)e^{-iqx}dx$. The [convolution theorem](../../../../../convolution-theorem.md) gives

$$
\boxed{\widehat{f*g}=\widehat f\,\widehat g},\qquad
\boxed{\widehat{fg}=\frac1{2\pi}\widehat f*\widehat g}.
$$

A finite array of very narrow slits at $x=jD$, $j=0,\ldots,N-1$, has transmission proportional to $\sum_j\delta(x-jD)$. It can be constructed by multiplying an infinite [Dirac comb](../../../../../dirac-comb.md) by a finite window. The infinite comb transforms to a reciprocal comb; the finite window convolves each reciprocal peak with a narrow sinc-shaped amplitude. Thus increasing the illuminated length narrows each [Fraunhofer diffraction](../../../../../fraunhofer-diffraction.md) peak.

The exact finite sum makes the argument quantitative:

$$
\widehat t(q)\propto\sum_{j=0}^{N-1}e^{-iqjD}
=e^{-iq(N-1)D/2}\frac{\sin(NqD/2)}{\sin(qD/2)},\qquad q=\frac{2\pi}{\lambda}\sin\theta.
$$

Its normalized intensity is $[\sin(NqD/2)/(N\sin(qD/2))]^2$. Principal maxima occur at $qD=2\pi m$; their first zeros are displaced by $|\Delta(qD)|=2\pi/N$. Replacing the ideal narrow slit by a finite slit function convolves the array in real space, multiplying this field by the single-slit [Fourier transform](../../../../../fourier-transform-split.md). Field amplitudes are transformed and combined before their squared modulus is taken.

<a id="section-b/b8/image-a-finite-narrow-slit-array-and-its-fourier-intensity-showing-how-the-principal-peaks-narrow-with-slit-count"></a>
![](../../../../../past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2017/paper-2-b8-finite-grating.png)

**[Figure 3](#section-b/b8/image-a-finite-narrow-slit-array-and-its-fourier-intensity-showing-how-the-principal-peaks-narrow-with-slit-count). A finite narrow-slit array and its Fourier intensity, showing how the principal peaks narrow with slit count**.

## ↑ Ancestors (15)

1. [Solution](solution.md)
2. [B8](../b8.md)
3. [Section B](../../section-b.md)
4. [Paper 2](../../../paper-2-split.md)
5. [2017](../../../split.md)
6. [Past exam of the physics A course of the University of Cambridge](../../../../split.md)
7. [Physics A course of the University of Cambridge](../../../../../physics-a-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../split.md)
