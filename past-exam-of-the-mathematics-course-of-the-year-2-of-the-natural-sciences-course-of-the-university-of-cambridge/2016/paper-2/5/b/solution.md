<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The inverse [Fourier transform](../../../../../fourier-transform-split.md) is

$$
f(t)=\frac1{2\pi}\int_{\mathbb R}\frac{-i\,e^{i\omega t}}{\omega-i}\,d\omega.
$$

For $t>0$, close in the upper half-plane, where $e^{i\omega t}$ decays. The single enclosed [pole](../../../../../pole.md) has [residue](../../../../../residue.md) $-ie^{-t}$, so counterclockwise integration gives $f=e^{-t}$. For $t<0$, close clockwise in the lower half-plane; there is no enclosed pole and the result is zero. Thus

$$
\boxed{f(t)=e^{-t}H(t),\qquad f(t)=0\ (t<0),\quad f(t)=e^{-t}\ (t>0).}
$$

Here $H$ is the [Heaviside step function](../../../../../heaviside-step-function.md). At the jump, symmetric [Fourier inversion](../../../../../fourier-inversion-theorem.md) gives $f(0)=1/2$, the average of the one-sided limits. The transform itself cannot fix a function’s value at a single point, so this is the conventional representative rather than extra frequency information.

A direct check is $\int_0^\infty e^{-(1+i\omega)t}dt=(1+i\omega)^{-1}=-i/(\omega-i)$. Distributionally, $f'=\delta(t)-e^{-t}H(t)$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 2](../../../paper-2-split.md)
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
