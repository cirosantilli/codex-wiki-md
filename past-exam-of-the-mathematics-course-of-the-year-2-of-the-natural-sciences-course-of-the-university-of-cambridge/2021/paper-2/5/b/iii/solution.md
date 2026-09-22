<h1 id="5/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Expand in the complete [Fourier sine series](../../../../../../fourier-sine-series.md) $\widetilde y(\omega,x)=\sum_{n\geq1}b_n(\omega)\sin(k_nx)$ and apply [Fourier inversion](../../../../../../fourier-inversion-theorem.md). Substitution of part (ii) gives

$$
\boxed{y(t,x)=\frac1{\pi L}\sum_{n=1}^\infty\sin(k_nx_0)\sin(k_nx)\int_{-\infty}^\infty\frac{\widetilde F(\omega)e^{i\omega t}}{k_n^2-\omega^2}\,d\omega,\qquad C=\frac1{\pi L}.}
$$

To check the source normalization, apply $\partial_t^2-\partial_x^2$ mode by mode. It cancels the denominator; the remaining inverse transform gives $2\pi F(t)$, and completeness gives

$$
\frac2L\sum_{n\geq1}\sin(k_nx_0)\sin(k_nx)=\delta(x-x_0).
$$

The endpoints vanish termwise. These identities establish the equation in the distributional sense, with classical validity wherever the series and derivatives converge suitably.

The displayed real-axis integrals in the paper are not ordinary convergent integrals at their [poles](../../../../../../pole.md). One definite choice is the [Cauchy principal value](../../../../../../cauchy-principal-value.md) at each $\omega=\pm k_n$. If a causal solution is wanted, use $[k_n^2-(\omega-i0)^2]^{-1}$ instead. Its inverse transform is $H(t)\sin(k_nt)/k_n$, so the causal solution is

$$
y_{\rm ret}(t,x)=\frac2L\sum_{n\geq1}\frac{\sin(k_nx_0)\sin(k_nx)}{k_n}\int_{-\infty}^tF(s)\sin[k_n(t-s)]\,ds,
$$

when the past integral exists. The principal-value choice instead uses the time-symmetric kernel $\sin(k_n|t|)/(2k_n)$. No temporal initial data are given, so homogeneous sine and cosine modes remain permissible additions. This is the [causal Fourier resolvent of a point-driven fixed string](../../../../../../causal-fourier-resolvent-of-a-point-driven-fixed-string.md).

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
