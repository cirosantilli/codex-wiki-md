<h1 id="3/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Reflecting repeatedly in the two parallel planes creates an infinite [method of images](../../../../../../method-of-images.md). For $\mathbf r'=(x',y',z')$, introduce

$$
\mathbf r_n^+=(x'+4n,y',z'),\qquad
\mathbf r_n^-=(-x'-2+4n,y',z'),\qquad n\in\mathbb Z.
$$

The [Dirichlet Green function between parallel planes](../../../../../../dirichlet-green-function-between-parallel-planes.md) is

$$
\boxed{G_{\rm slab}(\mathbf r,\mathbf r')=-\frac1{4\pi}\sum_{n\in\mathbb Z}
\left[\frac1{|\mathbf r-\mathbf r_n^+|}-\frac1{|\mathbf r-\mathbf r_n^-|}\right].}
$$

Each bracket is $O(n^{-2})$, so the paired series converges absolutely away from the sources. At $x=-1$, reflection pairs the positive image indexed by $n$ with the negative image indexed by $-n$. At $x=1$ it pairs that positive image with the negative image indexed by $1-n$. The distances agree in each pairing, making both boundary values zero. This can be checked with symmetric finite partial sums first; the unmatched end terms tend to zero, so no subtraction of separately divergent series is needed. Only $\mathbf r_0^+=\mathbf r'$ lies within the slab, so $\Delta_{\mathbf r}G_{\rm slab}=\delta(\mathbf r-\mathbf r')$. This is the usual Green function decaying at large transverse separation; such a condition selects the physical solution in the unbounded region.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
