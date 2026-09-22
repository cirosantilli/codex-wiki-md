<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $s(\theta)$ be the $2\pi$-periodic ramp represented by $\theta$ on $(-\pi,\pi)$. The [Fourier series of a periodic sawtooth](../../../../fourier-series-of-a-periodic-sawtooth.md) gives

$$
s(\theta)=2\sum_{n=1}^\infty\frac{(-1)^{n+1}}n\sin(n\theta).
$$

Both boundary data are multiples of this odd function, so their angular means and cosine coefficients vanish. Consequently $A_0=C_0=A_n=C_n=0$. Put $h_n=2(-1)^{n+1}/n$. Matching the sine coefficients at the two radii gives $B_na^n+D_na^{-n}=h_n\mu_a$ and $B_nb^n+D_nb^{-n}=h_n\mu_b$. Solving this two-by-two [linear system](../../../../system-of-linear-equations.md) yields

$$
\boxed{B_n=h_n\frac{\mu_bb^n-\mu_aa^n}{b^{2n}-a^{2n}},\qquad
D_n=h_n\frac{a^nb^n(\mu_ab^n-\mu_ba^n)}{b^{2n}-a^{2n}}.}
$$

Equivalently, [two-boundary annular harmonic interpolation](../../../../two-boundary-annular-harmonic-interpolation.md) expresses the same solution as

$$
\boxed{T(r,\theta)=\sum_{n=1}^\infty h_n\frac{\mu_a\sinh(n\log(b/r))+\mu_b\sinh(n\log(r/a))}{\sinh(n\log(b/a))}\sin(n\theta).}
$$

Every term is a [harmonic function](../../../../harmonic-function.md), and the radial factors enforce the specified boundary values. For a radius strictly between $a$ and $b$, their geometric decay makes the series smooth. At the boundary discontinuity $\theta=\pi$, the limiting Fourier value is the mean of the two one-sided values, zero. The boundary data are imposed away from that exceptional point, as stated.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [Paper 2](../../paper-2-split.md)
3. [2008](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
