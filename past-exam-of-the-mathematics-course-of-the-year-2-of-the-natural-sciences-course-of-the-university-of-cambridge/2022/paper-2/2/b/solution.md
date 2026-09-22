<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Project the [initial condition](../../../../../initial-condition.md) onto the orthogonal spatial [eigenfunctions](../../../../../eigenfunction.md). Their squared norms in the ordinary [inner product](../../../../../inner-product-split.md) are

$$
\int_0^1e^{2x}\,dx=\frac{e^2-1}{2},\qquad
\int_0^1V_n(x)^2\,dx=\frac{n^2\pi^2+1}{2}.
$$

The latter follows from the integrals of $\cos^2(n\pi x)$ and $\sin^2(n\pi x)$ being $1/2$, with the sine-cosine cross term zero. Therefore

$$
\boxed{c_0=\frac2{e^2-1}\int_0^1f(x)e^x\,dx,\qquad
c_n=\frac2{n^2\pi^2+1}\int_0^1f(x)\left[n\pi\cos(n\pi x)+\sin(n\pi x)\right]dx.}
$$

For square-integrable data the expansion converges to the data in the [L2 norm](../../../../../l2-norm.md) at $t=0$; for $t>0$ the decaying high modes are smoothed. Initial data with zero $e^x$ projection have no growing term.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
