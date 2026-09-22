<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Here $\lambda=7/2$ and $\alpha_n=n$. Let

$$
I_n=\int_0^\pi e^{-x}\sin(nx)\,dx,\qquad
J_n=\int_0^\pi e^{-x}\cos(nx)\,dx.
$$

Two applications of [integration by parts](../../../../../integration-by-parts.md) give

$$
I_n=nJ_n,\qquad
J_n=1-(-1)^ne^{-\pi}-nI_n.
$$

Solving these equations,

$$
I_n=\frac{n[1-(-1)^ne^{-\pi}]}{1+n^2},\qquad
f_n=\frac{2n[1-(-1)^ne^{-\pi}]}{\pi(1+n^2)}.
$$

Consequently the required amplitudes are

$$
\boxed{A_n=
\begin{cases}
\displaystyle\frac{2n[1-(-1)^ne^{-\pi}]}{\pi(1+n^2)\sqrt{49/4-n^2}},&1\leq n\leq3,\\[6pt]
\displaystyle\frac{2n[1-(-1)^ne^{-\pi}]}{\pi(1+n^2)\sqrt{n^2-49/4}},&n\geq4.
\end{cases}}
$$

The stated initial [velocity](../../../../../velocity.md) is nonzero at the fixed endpoints, whereas a classical solution differentiable there would require zero endpoint [velocity](../../../../../velocity.md). Thus it is understood on the open interval, or as an [L2 space](../../../../../l2-space-is-a-hilbert-space.md) initial datum in the usual finite-energy solution. Its [Fourier sine series](../../../../../fourier-sine-series.md) takes value zero at the endpoints; this changes no initial [energy](../../../../../energy-split.md) or interior initial data.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
