<h1 id="19/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take the spatial interval $0<x<L$ with $L>0$, and write $v=|c|>0$. A separated nonzero solution satisfies

$$
\frac{X''}{X}=\frac{T''}{v^2T}=-\lambda.
$$

The zero-endpoint [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md) rule out nonzero solutions for $\lambda\leq0$: linear or hyperbolic spatial factors cannot vanish at both ends. For $\lambda>0$, they give $X_n=\sin(n\pi x/L)$ and $\lambda_n=(n\pi/L)^2$, $n\geq1$. The temporal factors solve $T_n''+\omega_n^2T_n=0$, with the [fixed-end standing wave frequencies](../../../../../fixed-end-standing-wave-frequencies.md) $\omega_n=n\pi v/L$. Superposition gives

$$
\boxed{\psi(x,t)=\sum_{n=1}^{\infty}\left[A_n\cos\left(\frac{n\pi vt}{L}\right)+B_n\sin\left(\frac{n\pi vt}{L}\right)\right]\sin\left(\frac{n\pi x}{L}\right).}
$$

The constants are arbitrary subject to the convergence and regularity required of the solution. For initial displacement $f$ and initial [velocity](../../../../../velocity.md) $g$, their [Fourier sine series](../../../../../fourier-sine-series.md) give $A_n=(2/L)\int_0^Lf(x)\sin(n\pi x/L)dx$ and $B_n=(2/(L\omega_n))\int_0^Lg(x)\sin(n\pi x/L)dx$. Smooth compatible data give classical solutions; weaker data have the corresponding energy interpretation. A negative printed $L$ describes the interval with endpoints reversed and gives the same modes after using its positive length.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [19](../../19.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
