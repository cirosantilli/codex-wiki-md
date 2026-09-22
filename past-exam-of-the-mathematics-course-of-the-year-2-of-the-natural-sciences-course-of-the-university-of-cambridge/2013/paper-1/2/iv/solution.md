<h1 id="2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Let $d_n$ be the even [Fourier coefficient](../../../../../fourier-coefficient.md) of the initial displacement, with the normalization $\int_{-L}^L\cos^2(k_nx)dx=L$. Writing $s_n=\sin(n\pi/2)=(-1)^{(n-1)/2}$ gives

$$
\begin{aligned}
d_n&=\frac2L\int_0^Le^{-x/l}\cos(k_nx)\,dx\\
&=\boxed{\frac{2l}{L}\frac{1+k_nl\,s_ne^{-L/l}}{1+(k_nl)^2}}\qquad(n\text{ odd}).
\end{aligned}
$$

Zero initial velocity requires the real modal time factor

$$
T_n(t)=d_ne^{-\alpha t/2}\left[\cos(\omega_nt)+\frac{\alpha}{2\omega_n}\sin(\omega_nt)\right].
$$

One consistent choice in the question's complex representation is therefore

$$
\boxed{A_n=\frac{d_n}{2}\left(1-\frac{i\alpha}{2\omega_n}\right),\qquad B_n=\frac{d_n}{2}\left(1+\frac{i\alpha}{2\omega_n}\right).}
$$

For real $\omega_n$, $B_n=\overline{A_n}$; the real-part notation otherwise makes the complex coefficients nonunique. For imaginary $\omega_n$, the same formula is interpreted using [hyperbolic functions](../../../../../hyperbolic-function.md). Its limit at $\omega_n=0$ is $d_ne^{-\alpha t/2}(1+\alpha t/2)$.

For $l/L\to0$ at fixed mode number,

$$
\boxed{d_n\simeq\frac{2l/L}{1+(n\pi l/2L)^2},}
$$

which can be substituted into $A_n,B_n$ above. The profile specified at $t=0$ is actually nonzero at $x=\pm L$. Thus for finite $l/L$ it cannot be the initial data of a solution continuous at the initial endpoint corners with fixed endpoints. The [Fourier series](../../../../../fourier-series-split.md) reproduces it in the open interval, with zero endpoint values; it is an [L2 space](../../../../../l2-space-is-a-hilbert-space.md) initial-data interpretation. The assumption $l\ll L$ makes this compatibility error exponentially small, rather than exactly zero.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
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
