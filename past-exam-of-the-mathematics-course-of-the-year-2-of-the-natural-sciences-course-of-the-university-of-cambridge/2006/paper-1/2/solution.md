<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

[Separation of variables](../../../../separation-of-variables.md) in the [wave equation](../../../../wave-equation-split.md) with fixed endpoints selects $H_n(x)=\sin(n\pi x/L)$ and angular frequencies $\omega_n=cn\pi/L$, $n\geq1$. The time factors may be chosen as $F_n(t)=\cos\omega_nt$, $G_n(t)=\sin\omega_nt$. By [Fourier sine series](../../../../fourier-sine-series.md) orthogonality, the initial data give

$$
a_n=\frac2L\int_0^Lf(x)\sin\frac{n\pi x}{L}\,dx,\qquad b_n=\frac2{L\omega_n}\int_0^Lg(x)\sin\frac{n\pi x}{L}\,dx.
$$

Hence $u=\sum_{n\geq1}[a_n\cos\omega_nt+b_n\sin\omega_nt]\sin(n\pi x/L)$. The factor $1/\omega_n$ in $b_n$ is required because differentiating the time sine supplies $\omega_n$.

The given displacement is a symmetric triangular tent: it is zero at both endpoints and has height $k$ at $L/2$. Integrating each linear half gives $a_n=8k\sin(n\pi/2)/(n^2\pi^2)$. Release from rest gives $b_n=0$, so the [midpoint-plucked fixed-end string](../../../../midpoint-plucked-fixed-end-string.md) is

$$
\boxed{u(x,t)=\frac{8k}{\pi^2}\sum_{m=0}^\infty\frac{(-1)^m}{(2m+1)^2}\cos\frac{(2m+1)\pi ct}{L}\sin\frac{(2m+1)\pi x}{L}.}
$$

Only odd modes occur, by symmetry about the midpoint. The initial slope corner makes this a finite-energy [weak solution](../../../../weak-solution.md); it is a classical solution away from the propagating corner lines.

<a id="2/image-initial-triangular-pluck-and-later-shapes-of-a-fixed-end-string"></a>
![](../../../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2006/paper-1-plucked-string.png)

**[Figure 1](#2/image-initial-triangular-pluck-and-later-shapes-of-a-fixed-end-string). Initial triangular pluck and later shapes of a fixed-end string**. Original normalized displacement and modal predictions. The initial tent reaches one at the midpoint; snapshots use time $ct/L$. The string passes through a straight configuration at $ct/L=1/2$ and reverses its initial displacement at $ct/L=1$.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [Paper 1](../../paper-1-split.md)
3. [2006](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
