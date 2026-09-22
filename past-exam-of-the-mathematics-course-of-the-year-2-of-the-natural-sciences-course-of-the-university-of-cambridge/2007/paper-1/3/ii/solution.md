<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Take the spatial [Fourier transform](../../../../../fourier-transform-split.md) with the same convention. The [partial differential equation](../../../../../partial-differential-equation-split.md) becomes $i\partial_t\widehat f-k^2\widehat f=0$, so $\widehat f(k,t)=e^{-ik^2t}\widehat f_0(k)$. Inverting and substituting the transform of the initial [function](../../../../../function-split.md) yields the [convolution](../../../../../convolution.md)

$$
f(x,t)=\int_{\mathbb R}f_0(\xi)K_t(x-\xi)d\xi,\qquad K_t(s)=\frac1{2\pi}\int_{\mathbb R}e^{iks-itk^2}dk.
$$

Complete the square, $iks-itk^2=is^2/(4t)-it[k-s/(2t)]^2$, and put $\ell=\sqrt t[k-s/(2t)]$. This gives

$$
\boxed{f(x,t)=\frac{c}{2\pi\sqrt t}\int_{-\infty}^{\infty}f_0(\xi)e^{i(x-\xi)^2/(4t)}d\xi,\qquad c=\int_{\mathbb R}e^{-i\ell^2}d\ell=\sqrt\pi e^{-i\pi/4}.}
$$

The oscillatory Gaussian is a [Fresnel integral](../../../../../fresnel-integral.md), understood as the limit with a positive Gaussian damping factor. That prescription also justifies the transform manipulations, first for rapidly decreasing smooth data and then by [L2 space](../../../../../l2-space-is-a-hilbert-space.md) extension. The resulting kernel is the [free-particle propagator](../../../../../free-particle-propagator.md) in units $\hbar=1$, $m=1/2$; its phase and normalization agree with the multiplier $e^{-ik^2t}$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
