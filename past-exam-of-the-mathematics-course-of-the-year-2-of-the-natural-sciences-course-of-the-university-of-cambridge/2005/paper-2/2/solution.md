<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Set $\phi=R(r)\Theta(\theta)$ in [Laplace's equation](../../../../laplace-equation.md). Separation gives $\Theta''+n^2\Theta=0$ and $r^2R''+rR'-n^2R=0$. Single-valued angular periodicity requires integer $n\geq0$. For $n>0$ the radial factors are $r^n,r^{-n}$; for $n=0$ they are $1,\ln r$. A term linear in $\theta$ is excluded by periodicity. Thus the [harmonic Fourier expansions in planar concentric domains](../../../../harmonic-fourier-expansions-in-planar-concentric-domains.md) have the general form

$$
\phi=A+B\ln r+\sum_{n\geq1}[r^n(A_n\cos n\theta+B_n\sin n\theta)+r^{-n}(C_n\cos n\theta+D_n\sin n\theta)].
$$

For $0<a<b$, the specified boundaries contain only a constant mode and a first cosine mode. The [two-boundary annular harmonic interpolation](../../../../two-boundary-annular-harmonic-interpolation.md) gives

$$
\boxed{\phi(r,\theta)=U\frac{\ln(b/r)}{\ln(b/a)}+V\frac{b}{b^2-a^2}\left(r-\frac{a^2}{r}\right)\cos\theta.}
$$

At $r=a$, the cosine term vanishes and the logarithmic term is $U$; at $r=b$, the first term vanishes and the cosine amplitude is $V$. Each component is harmonic, and the [maximum principle](../../../../maximum-principle.md) ensures uniqueness for these continuous [Dirichlet boundary conditions](../../../../dirichlet-boundary-condition.md).

## ↑ Ancestors (12)

1. [2](../2.md)
2. [Paper 2](../../paper-2-split.md)
3. [2005](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
