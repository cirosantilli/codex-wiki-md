<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For each sine [normal mode](../../../../../normal-mode.md), the temporal [characteristic equation](../../../../../characteristic-equation-of-a-constant-coefficient-differential-equation.md) is $s^2+2\lambda s+\alpha_n^2=0$, with roots $s=-\lambda\pm\sqrt{\lambda^2-\alpha_n^2}$. Since $\lambda L/\pi=M+1/2$, the first $M$ modes are [overdamped](../../../../../overdamping.md) and all higher modes are [underdamped](../../../../../underdamping.md). No integer $n$ gives [critical damping](../../../../../critical-damping.md).

The zero initial displacement excludes the hyperbolic cosine and cosine terms. Hence

$$
\begin{aligned}
u(x,t)=e^{-\lambda t}\bigg[&\sum_{n=1}^{M}A_n\sin(\alpha_nx)\sinh(\Omega_nt)\\
&+\sum_{n=M+1}^{\infty}A_n\sin(\alpha_nx)\sin(\omega_nt)\bigg],
\end{aligned}
$$

where

$$
\boxed{\begin{aligned}
\alpha_n&=\frac{n\pi}{L},\\
\Omega_n&=\frac\pi L\sqrt{\left(M+\frac12\right)^2-n^2}\quad(1\leq n\leq M),\\
\omega_n&=\frac\pi L\sqrt{n^2-\left(M+\frac12\right)^2}\quad(n\geq M+1).
\end{aligned}}
$$

To impose the initial [velocity](../../../../../velocity.md), let $f_n=\frac2L\int_0^L f(x)\sin(\alpha_nx)\,dx$ be its [Fourier sine series](../../../../../fourier-sine-series.md) coefficients. Differentiating the expansion at $t=0$ gives $A_n\Omega_n=f_n$ for the [overdamped](../../../../../overdamping.md) modes and $A_n\omega_n=f_n$ for the [underdamped](../../../../../underdamping.md) modes. These determine all coefficients. Despite the hyperbolic sine, the first modes decay: $\Omega_n<\lambda$, so both temporal exponential rates are negative.

## ↑ Ancestors (13)

1. [B](../b.md)
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
