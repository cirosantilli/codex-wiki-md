<h1 id="18/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For fixed $r<1$, $\sum r^n\cos(n\theta)$ converges absolutely and uniformly. Thus for integrable $f$, one may integrate the kernel [series](../../../../../series-mathematics.md) term by term. The [cosine addition formula](../../../../../cosine-addition-formula.md) gives

$$
\cos[n(\theta-t)]=\cos(n\theta)\cos(nt)+\sin(n\theta)\sin(nt).
$$

Substitute this into the defining [integral](../../../../../integral-split.md). The constant kernel term gives $\tfrac1{2\pi}\int f=a_0/2$; the remaining terms give

$$
\boxed{y_f(r,\theta)=\frac{a_0}{2}+\sum_{n=1}^\infty r^n[a_n\cos(n\theta)+b_n\sin(n\theta)],}
$$

where

$$
\boxed{a_n=\frac1\pi\int_{-\pi}^{\pi}f(t)\cos(nt)\,dt,\qquad
b_n=\frac1\pi\int_{-\pi}^{\pi}f(t)\sin(nt)\,dt.}
$$

These are the same [Fourier coefficients](../../../../../fourier-coefficient.md) as in part (a). The kernel $2K$ is the [Poisson kernel for the unit disk](../../../../../poisson-kernel-for-the-unit-disk.md); the factors $r^n$ suppress the higher angular frequencies inside the [disk](../../../../../disk-mathematics.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [18](../../18.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
