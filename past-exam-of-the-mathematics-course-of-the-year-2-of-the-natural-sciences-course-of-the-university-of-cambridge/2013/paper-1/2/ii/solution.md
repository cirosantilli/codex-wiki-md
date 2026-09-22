<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

An [even function](../../../../../even-function.md) satisfying the spatial equation has $X=C\cos(kx)$. The [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md) require $\cos(kL)=0$, so the allowed [wavenumbers](../../../../../wavenumber.md) are

$$
k_n=\frac{n\pi}{2L},\qquad n=1,3,5,\ldots.
$$

There is no nonzero zero-wavenumber mode. With $T=e^{-\alpha t/2}S$, the time equation becomes $S''+\omega_n^2S=0$, where $\omega_n^2=c^2k_n^2-\alpha^2/4$. Thus [superposition](../../../../../superposition-principle.md) of the even [normal modes](../../../../../normal-mode.md) gives

$$
\boxed{u(x,t)=\sum_{\substack{n\geq1\\ n\ {
m odd}}}e^{-\alpha t/2}\cos(k_nx)\operatorname{Re}\left(A_ne^{i\omega_nt}+B_ne^{-i\omega_nt}\right).}
$$

This uses completeness of the even [Fourier series](../../../../../fourier-series-split.md) modes. Imaginary $\omega_n$ describe [overdamping](../../../../../overdamping.md). At [critical damping](../../../../../critical-damping.md), $\omega_n=0$, the two displayed exponentials coincide: the complete time factor must instead be $e^{-\alpha t/2}(C_n+D_nt)$. This repeated-root exception is necessary for a genuinely general solution.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
