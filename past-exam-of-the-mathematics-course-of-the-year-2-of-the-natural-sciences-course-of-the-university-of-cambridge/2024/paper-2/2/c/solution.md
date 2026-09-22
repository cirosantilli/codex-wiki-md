<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Reflecting the solution across $\theta=\pi\alpha$ preserves its [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md) and outer boundary data, so uniqueness makes the solution reflection-symmetric. Since

$$
\sin\frac{n(2\pi\alpha-\theta)}{2\alpha}=(-1)^{n+1}\sin\frac{n\theta}{2\alpha},
$$

only odd angular [Fourier modes](../../../../../fourier-mode.md) survive. Put $\rho=(r/R)^{1/(2\alpha)}$ and $\psi=\theta/(2\alpha)$. On the symmetry axis $\psi=\pi/2$, comparison of the convergent [power series](../../../../../power-series.md) gives

$$
A_{2j+1}R^{(2j+1)/(2\alpha)}(-1)^j=\frac1{(2j+1)!}.
$$

Thus

$$
\boxed{\Phi(r,\theta)=\sum_{j=0}^{\infty}\frac{(-1)^j\rho^{2j+1}}{(2j+1)!}\sin\bigl((2j+1)\psi\bigr).}
$$

This is the [imaginary part](../../../../../imaginary-part.md) of $\sin(\rho e^{i\psi})$, so a useful closed form is

$$
\boxed{\Phi(r,\theta)=\cos\bigl(\rho\cos\psi\bigr)\sinh\bigl(\rho\sin\psi\bigr).}
$$

At either straight edge $\sin\psi=0$, while on the symmetry axis the formula is $\sinh\rho$. Every term is [harmonic](../../../../../harmonic-function.md) in the sector, and the factorial denominator gives convergence up to $r=R$, verifying the full solution.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
