<h1 id="18/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The boundary data are odd except at isolated endpoint choices, which do not change [integrals](../../../../../integral-split.md). Thus every cosine [Fourier coefficient](../../../../../fourier-coefficient.md), including $a_0$, vanishes. For the sine [Fourier coefficients](../../../../../fourier-coefficient.md),

$$
b_n=\frac2\pi\int_0^\pi\sin(nt)\,dt=\frac{2[1-(-1)^n]}{\pi n}
=\begin{cases}4/(\pi n),&n\text{ odd},\\0,&n\text{ even}.\end{cases}
$$

Consequently the extension is

$$
\boxed{y_{f_0}(r,\theta)=\frac4\pi\sum_{\substack{n\ge1\\n\text{ odd}}}\frac{r^n\sin(n\theta)}n.}
$$

It converges absolutely for every $r<1$; its limiting boundary values at jumps are the midpoint of the two one-sided limits.

## ↑ Ancestors (13)

1. [C](../c.md)
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
