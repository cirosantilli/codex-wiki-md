<h1 id="17/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume $L>0$. For any nonzero integer $k$,

$$
\int_{-L}^{L}\cos(k\pi x/L)\,dx
=\frac{L}{k\pi}[\sin(k\pi x/L)]_{-L}^{L}=0.
$$

For $m\ne n$, the product-to-sum identity expresses the integrand as one half the sum of cosines with nonzero frequencies $m-n$ and $m+n$, so the integral is zero. For $m=n>0$, use $\cos^2u=(1+\cos2u)/2$ to get $L$. Finally, for $m=n=0$ the integrand is one. The complete [Fourier orthogonality](../../../../../fourier-orthogonality.md) formula is

$$
\boxed{\int_{-L}^{L}\cos\frac{m\pi x}{L}\cos\frac{n\pi x}{L}\,dx
=\begin{cases}2L,&m=n=0,\\L,&m=n\geq1,\\0,&m\ne n.\end{cases}}
$$

The constant mode has twice the squared norm of a positive-frequency [cosine](../../../../../cosine.md) mode.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [17](../../17.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
