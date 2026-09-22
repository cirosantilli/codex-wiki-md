<h1 id="17/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $h_n=a_n\cos(n\pi x/L)+b_n\sin(n\pi x/L)$. For the partial sum $S_N=a_0/2+\sum_{n=1}^Nh_n$, ordinary multiplication gives

$$
S_N^2=\frac{a_0^2}4+a_0\sum_{n=1}^Nh_n+\sum_{m,n=1}^Nh_mh_n.
$$

On $[-L,L]$, the integrals of every nonconstant sine or cosine vanish. [Fourier orthogonality](../../../../../fourier-orthogonality.md) further gives $\int\cos(m\pi x/L)\cos(n\pi x/L)dx=L\delta_{mn}$ and the same identity for two sines, while every sine-cosine integral is zero. Thus

$$
\frac1{2L}\int_{-L}^LS_N^2dx=\frac{a_0^2}4+\frac12\sum_{n=1}^N(a_n^2+b_n^2).
$$

For square-integrable $f$, its [Fourier partial sums](../../../../../fourier-partial-sum.md) converge to $f$ in [L2 space](../../../../../l2-space-is-a-hilbert-space.md), so their squared norms converge to the squared norm of $f$. Passing to the limit proves [Parseval's identity](../../../../../parseval-identity.md):

$$
\boxed{\frac1T\int_{-T/2}^{T/2}f(x)^2dx=\left(\frac{a_0}2\right)^2+\frac12\sum_{n=1}^{\infty}(a_n^2+b_n^2).}
$$

Working with finite partial sums before taking the norm limit avoids an unjustified interchange of an infinite double series and integration.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [17](../../17.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
