<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use [separation of variables](../../../../separation-of-variables.md) $u=X(x)T(t)$. The fixed-end [Dirichlet boundary conditions](../../../../dirichlet-boundary-condition.md) select $X_n=\sin(nx)$, $n\geq1$, and each mode satisfies $T_n''+2hT_n'+n^2T_n=0$. In the physical resistance range $0\leq h<1$, all [normal modes](../../../../normal-mode.md) are underdamped, with $\omega_n=\sqrt{n^2-h^2}>0$. The modal factor normalized by $T_n(0)=1$, $T_n'(0)=0$ is

$$
T_n(t)=e^{-ht}\left[\cos(\omega_nt)+\frac h{\omega_n}\sin(\omega_nt)\right].
$$

Consequently the [linearly damped string](../../../../linearly-damped-string.md) has solution

$$
\boxed{u(x,t)=\sum_{n=1}^\infty b_n\sin(nx)e^{-ht}\left[\cos(\omega_nt)+\frac h{\omega_n}\sin(\omega_nt)\right],\quad b_n=\frac2\pi\int_0^\pi f(x)\sin(nx)dx.}
$$

The coefficients are those of the initial [Fourier sine series](../../../../fourier-sine-series.md). Differentiating each normalized modal factor at zero confirms that the string starts from rest. Suitable initial data give convergence in the string's energy space; the piecewise linear profile here need not give a twice differentiable solution along every characteristic from its corner.

For the specified tent profile, integrating its two linear pieces by parts gives

$$
\int_0^\pi f(x)\sin(nx)dx=\frac{2}{n^2}\sin\frac{n\pi}{2}.
$$

For example the first piece gives $-\pi\cos(n\pi/2)/(2n)+\sin(n\pi/2)/n^2$, and the second gives the opposite cosine term and the same sine term. Hence

$$
\boxed{b_n=\frac4{\pi n^2}\sin\frac{n\pi}{2},\qquad b_{2m}=0,\quad b_{2m+1}=\frac{4(-1)^m}{\pi(2m+1)^2}.}
$$

The zero even coefficients also follow from reflection symmetry about the midpoint. This is the [Fourier sine series of a symmetric tent](../../../../fourier-sine-series-of-a-symmetric-tent.md). If $h<1$ were read without the physical assumption $h\geq0$, the same modal solution extends by replacing imaginary-frequency sine and cosine by their hyperbolic counterparts, and taking $\sin(\omega t)/\omega=t$ when $\omega=0$.

<a id="2/image-evolution-of-a-tent-shaped-string-released-from-rest-with-linear-damping"></a>
![](../../../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2009/paper-1-damped-tent-string.png)

**[Figure 1](#2/image-evolution-of-a-tent-shaped-string-released-from-rest-with-linear-damping). Evolution of a tent-shaped string released from rest with linear damping**.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [Paper 1](../../paper-1-split.md)
3. [2009](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
