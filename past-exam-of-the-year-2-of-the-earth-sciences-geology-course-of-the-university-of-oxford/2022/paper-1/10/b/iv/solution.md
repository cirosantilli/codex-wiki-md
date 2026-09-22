<h1 id="10/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For an integrable initial profile $f(y)$, use its [Fourier transform](../../../../../../fourier-transform-split.md) with the convention

$$
\widehat f(k)=\int_{\mathbb R}f(y)e^{-iky}\,dy.
$$

The transformed [diffusion equation](../../../../../../diffusion-equation-split.md) is $\partial_t\widehat T=-\kappa k^2\widehat T$, so

$$
\boxed{T(t,y)=\frac1{2\pi}\int_{\mathbb R}\widehat f(k)e^{-\kappa k^2t}e^{iky}\,dk.}
$$

Equivalently the [heat-kernel convolution](../../../../../../heat-kernel-convolution.md) is

$$
T(t,y)=\frac1{\sqrt{4\pi\kappa t}}\int_{\mathbb R}
\exp\!\left[-\frac{(y-\eta)^2}{4\kappa t}\right]f(\eta)\,d\eta.
$$

This also accommodates bounded piecewise-continuous initial profiles; it recovers $f$ at continuity points as $t\downarrow0$. For periodic initial data use a [Fourier series](../../../../../../fourier-series-split.md) and multiply each mode by $e^{-\kappa k_r^2t}$; the constant mean mode remains unchanged. “Any function” needs the usual existence/integrability or growth conditions: an arbitrarily fast-growing initial function need not give a finite heat-kernel integral.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [10](../../../10.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the year 2 of the earth sciences (geology) course of the University of Oxford](../../../../../split.md)
7. [Year 2 of the earth sciences (geology) course of the University of Oxford](../../../../../../year-2-of-the-earth-sciences-geology-course-of-the-university-of-oxford.md)
8. [Earth sciences (geology) course of the University of Oxford](../../../../../../earth-sciences-geology-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
