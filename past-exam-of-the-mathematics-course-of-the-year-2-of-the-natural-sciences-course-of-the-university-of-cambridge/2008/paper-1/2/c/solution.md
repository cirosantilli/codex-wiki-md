<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Each spatial [eigenfunction](../../../../../eigenfunction.md) acquires the temporal factor $e^{-\kappa\lambda_{mn}t}$ under the [heat equation](../../../../../heat-equation.md). Expanding the initial constant using the preceding coefficients gives the [cooling of an initially uniform square](../../../../../cooling-of-an-initially-uniform-square.md):

$$
\boxed{T(x,y;t)=\frac{16T_0}{\pi^2}\sum_{\substack{m,n\geq1\\m,n\text{ odd}}}\frac1{mn}\sin\frac{m\pi x}{\ell}\sin\frac{n\pi y}{\ell}\,e^{-\kappa\pi^2(m^2+n^2)t/\ell^2}.}
$$

For $t>0$ the exponential factors justify differentiating the series and enforce the zero boundary temperature. As $t\downarrow0$, it tends to $T_0$ at every interior point and in [L2 space](../../../../../l2-space-is-a-hilbert-space.md); the instantaneous boundary cooling is incompatible with continuity at the initial boundary corners, which is expected for this idealization.

The slowest decaying nonzero mode is $(1,1)$, giving

$$
\boxed{T(x,y;t)\sim\frac{16T_0}{\pi^2}\sin\frac{\pi x}{\ell}\sin\frac{\pi y}{\ell}\,e^{-2\kappa\pi^2t/\ell^2}}
$$

at each fixed interior point when $T_0\ne0$. The next contributing modes have $(m,n)=(1,3),(3,1)$ and decay as $e^{-10\kappa\pi^2t/\ell^2}$, making the leading-mode approximation exponentially accurate.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
