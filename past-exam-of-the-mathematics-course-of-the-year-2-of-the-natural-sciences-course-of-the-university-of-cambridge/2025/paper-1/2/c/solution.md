<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [separation of variables](../../../../../separation-of-variables.md) solution with [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md) on the cuboid is

$$
\boxed{n=\sum_{p,q,r\geq1}a_{p,q,r}\sin\frac{p\pi x}{\lambda L}\sin\frac{q\pi\sqrt\lambda\,y}{L}\sin\frac{r\pi\sqrt\lambda\,z}{L}\exp\left\{\left[\gamma-\frac{\mu\pi^2}{L^2}\left(\frac{p^2}{\lambda^2}+\lambda q^2+\lambda r^2\right)\right]t\right\}.}
$$

The constants are fixed by the initial density through [Fourier sine series](../../../../../fourier-sine-series.md). The fastest term again has $p=q=r=1$. When $L=2L_{\mathrm{crit}}$, its growth rate becomes

$$
s_{111}=\gamma\left[1-\frac1{12}(\lambda^{-2}+2\lambda)\right].
$$

Thus the precise condition for no exponentially growing term is

$$
\boxed{\lambda^{-2}+2\lambda\geq12,\qquad\text{equivalently }2\lambda^3-12\lambda^2+1\geq0,\quad\lambda>0.}
$$

For example, $\lambda=1/4$ gives $\lambda^{-2}+2\lambda=33/2>12$, while $\lambda=6$ gives $12+1/36>12$: either a sufficiently flat or a sufficiently elongated cuboid suppresses growth despite its unchanged volume. The function $\lambda^{-2}+2\lambda$ decreases to its minimum $3$ at $\lambda=1$, then increases without bound. Hence there are two positive threshold values, with growth only between them; equality leaves one stationary term and all other terms decaying.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
