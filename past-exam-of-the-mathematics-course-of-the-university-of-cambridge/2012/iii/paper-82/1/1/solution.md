<h1 id="1/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [Fejér kernel](../../../../../../fejer-kernel.md) for the printed normalization is

$$
F_N(t)=\frac1N\left|\sum_{j=0}^{N-1}e^{2\pi ijt}\right|^2
=\sum_{|j|\le N}\left(1-\frac{|j|}{N}\right)e^{2\pi ijt}.
$$

Its endpoint coefficients at $\pm N$ are zero. It is nonnegative, and integrating its [Fourier series](../../../../../../fourier-series-split.md) gives $\int_{\mathbb T}F_N=1$. Hence $\widetilde S_N(f)=f*F_N$ and

$$
|\widetilde S_N(f,t)|\le\|f\|_\infty\int F_N\le1,
\qquad\boxed{\widetilde S^*(f,t)\le1.}
$$

Thus **the absolute constant can be $C=1$**. Positivity of the [Fejér kernel](../../../../../../fejer-kernel.md), rather than mere boundedness of its individual [Fourier coefficients](../../../../../../fourier-coefficient.md), is the reason this holds.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [1](../../1.md)
3. [Section A](../../section-a.md)
4. [Paper 82](../../../paper-82-split.md)
5. [Iii](../../../split.md)
6. [2012](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
