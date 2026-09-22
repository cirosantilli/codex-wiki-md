<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

First decompose the initial $y$ dependence using $\sin^2(2\pi y/b)=[1-\cos(4\pi y/b)]/2$. Only the cosine indices $m=0$ and $m=4$ occur. Expand the remaining factor in a [Fourier sine series](../../../../../fourier-sine-series.md):

$$
x(a-x)=\sum_{n=1}^\infty b_n\sin\frac{n\pi x}{a},\qquad b_n=\frac2a\int_0^ax(a-x)\sin\frac{n\pi x}{a}\,dx.
$$

For $k_n=n\pi/a$, two [integrations by parts](../../../../../integration-by-parts.md) give

$$
\int_0^ax(a-x)\sin(k_nx)dx=\frac{2[1-(-1)^n]}{k_n^3},\qquad b_n=\frac{4a^2[1-(-1)^n]}{n^3\pi^3}.
$$

Thus even $n$ vanish, while $b_n=8a^2/(n^3\pi^3)$ for odd $n$. The nonzero double-series coefficients are $A_{n0}=b_n/2$ and $A_{n4}=-b_n/2$. Their separate heat-mode decay factors give

$$
\boxed{T(x,y,t)=\frac{4a^2}{\pi^3}\sum_{\substack{n\geq1\\n\text{ odd}}}\frac{\sin(n\pi x/a)}{n^3}e^{-\lambda\pi^2n^2t/a^2}\left[1-e^{-16\lambda\pi^2t/b^2}\cos\frac{4\pi y}{b}\right].}
$$

At $t=0$ the bracket is $2\sin^2(2\pi y/b)$, which recovers the initial profile with the displayed sine coefficients. Each term satisfies the mixed [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md) and [Neumann boundary conditions](../../../../../neumann-boundary-condition.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
