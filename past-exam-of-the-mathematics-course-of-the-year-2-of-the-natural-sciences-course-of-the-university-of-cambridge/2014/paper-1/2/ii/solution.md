<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Separate variables as $u=X(x)T(t)$. The zero values at both plates give the [Fourier sine basis](../../../../../fourier-sine-basis.md)

$$
X_j(x)=\sin\frac{j\pi x}{L},\qquad T_j(t)=e^{-\nu j^2\pi^2t/L^2},\qquad j\geq1.
$$

Expand the initial profile using [orthogonality](../../../../../orthogonal-vectors.md). With $s=x/L$, its coefficients are

$$
A_j=\frac2L\int_0^LU_0\left(\frac xL-\frac{x^2}{L^2}\right)\sin\frac{j\pi x}{L}\,dx=2U_0\int_0^1s(1-s)\sin(j\pi s)\,ds=\frac{4U_0[1-(-1)^j]}{j^3\pi^3}.
$$

Consequently

$$
\boxed{u(x,t)=\frac{8U_0}{\pi^3}\sum_{\substack{j\geq1\\j\ {
m odd}}}\frac{\sin(j\pi x/L)}{j^3}e^{-\nu j^2\pi^2t/L^2}.}
$$

Only odd modes occur because the initial profile is symmetric about the midpoint. The coefficients are absolutely summable, so [dominated convergence](../../../../../dominated-convergence-theorem.md) gives $\boxed{u(x,t)\to0}$ uniformly as $t\to\infty$. The slowest decay rate is $\nu\pi^2/L^2$, associated with $j=1$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
