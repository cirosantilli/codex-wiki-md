<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a separated [harmonic function](../../../../../harmonic-function.md) $R(r)\Theta(\theta)$ in [polar coordinates](../../../../../polar-coordinates.md), single-valuedness forces integer angular frequencies. The radial factors for frequency $m\geq1$ are $r^m,r^{-m}$, while frequency zero has a constant and $\ln r$. Finiteness at the origin excludes $r^{-m}$ and $\ln r$.

The source's angular factor is $\cos\theta$ in every term, as printed, rather than $\cos(n\theta)$. The [power-law angular mode for the planar Poisson equation](../../../../../power-law-angular-mode-for-the-planar-poisson-equation.md) gives

$$
\Delta[r^{n+2}\cos\theta]=[(n+2)^2-1]r^n\cos\theta=(n+1)(n+3)r^n\cos\theta.
$$

Hence, assuming the series permits termwise differentiation, the general finite, single-valued solution is

$$
\boxed{\phi=C+\sum_{m=1}^\infty r^m[A_m\cos(m\theta)+B_m\sin(m\theta)]+\cos\theta\sum_{n=0}^\infty\frac{\alpha_n r^{n+2}}{(n+1)(n+3)}.}
$$

The arbitrary harmonic series must itself converge to a finite function on the prescribed disk. If $\alpha_0\ne0$, the source has a direction-dependent limit at the origin; the displayed potential still extends finitely there, but the equation at that point is understood weakly rather than as a smooth classical source.

For the special source, a particular potential is $r^3\cos\theta/8$. Its boundary cosine term is canceled by $-a^2r\cos\theta/8$, and the boundary sine term is supplied by $(r/a)^2\sin2\theta$. The resulting [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md) has solution

$$
\boxed{\phi(r,\theta)=\frac{r(r^2-a^2)}8\cos\theta+\frac{r^2}{a^2}\sin2\theta.}
$$

It is finite at zero, has the required boundary values, and its [Laplacian](../../../../../laplacian.md) is $r\cos\theta$.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
