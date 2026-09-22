<h1 id="7/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $n\geq2$ be even and integrate $f(z)=1/(1+z^n)$ around an upper-half-plane [semicircle](../../../../../semicircle.md) of radius $R>1$ with the real segment traversed from $-R$ to $R$. There are no real [poles](../../../../../pole.md), and the $n/2$ upper-half-plane [poles](../../../../../pole.md) are

$$
z_j=e^{i(2j+1)\pi/n},\qquad j=0,\ldots,n/2-1.
$$

Each is simple. Since $z_j^n=-1$,

$$
\operatorname{Res}_{z=z_j}f=\frac1{nz_j^{n-1}}=-\frac{z_j}{n}.
$$

On the [semicircle](../../../../../semicircle.md) the [integral](../../../../../integral-split.md) magnitude is at most $\pi R/(R^n-1)$, which tends to zero. The real [integral](../../../../../integral-split.md) is [absolutely convergent](../../../../../absolute-convergence.md) because its tail is of order $|x|^{-n}$. Thus

$$
\int_{-\infty}^{\infty}\frac{dx}{1+x^n}
=-\frac{2\pi i}{n}\sum_{j=0}^{n/2-1}e^{i(2j+1)\pi/n}.
$$

Evaluate the finite [geometric series](../../../../../geometric-series.md), writing $\theta=\pi/n$:

$$
\sum_{j=0}^{n/2-1}e^{i(2j+1)\theta}
=e^{i\theta}\frac{1-e^{in\theta}}{1-e^{2i\theta}}
=\frac{2e^{i\theta}}{-2ie^{i\theta}\sin\theta}
=\frac{i}{\sin\theta}.
$$

Consequently

$$
\boxed{\int_{-\infty}^{\infty}\frac{dx}{1+x^n}=\frac{2\pi}{n\sin(\pi/n)},\qquad
A_n=\frac{2\pi}{n},\quad B_n=\frac\pi n.}
$$

For $n=2$ this reduces to $\pi$, as a check on the contour orientation and [residue](../../../../../residue.md) signs.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [7](../../7.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
