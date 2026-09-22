<h1 id="18/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [Fourier series](../../../../../fourier-series-split.md) represents a periodic [function](../../../../../function-split.md) as a constant plus [sine](../../../../../sine.md) and [cosine](../../../../../cosine.md) waves whose frequencies are integer multiples of its fundamental frequency. For period $2L$, use the convention

$$
f(x)\sim\frac{a_0}{2}+\sum_{n=1}^{\infty}\left[a_n\cos\left(\frac{n\pi x}{L}\right)+b_n\sin\left(\frac{n\pi x}{L}\right)\right],
$$

where the [Fourier coefficients](../../../../../fourier-coefficient.md) are

$$
\boxed{\begin{aligned}
a_0&=\frac1L\int_{-L}^{L}f(x)\,dx,\\
a_n&=\frac1L\int_{-L}^{L}f(x)\cos\left(\frac{n\pi x}{L}\right)\,dx,\quad n\geq1,\\
b_n&=\frac1L\int_{-L}^{L}f(x)\sin\left(\frac{n\pi x}{L}\right)\,dx,\quad n\geq1.
\end{aligned}}
$$

The coefficient formulas follow by multiplying by a basis [sine](../../../../../sine.md) or [cosine](../../../../../cosine.md) and using their [orthogonality](../../../../../orthogonal-vectors.md) over a full period. A [Fourier series](../../../../../fourier-series-split.md) need not equal an arbitrary [function](../../../../../function-split.md) at every [point](../../../../../point-geometry.md). The [pointwise convergence of a piecewise smooth Fourier series](../../../../../pointwise-convergence-of-a-piecewise-smooth-fourier-series.md) theorem says that for a piecewise continuously differentiable [function](../../../../../function-split.md), the [Fourier series](../../../../../fourier-series-split.md) converges at each [point](../../../../../point-geometry.md) to the average of the two one-sided limits, and hence to $f(x)$ wherever $f$ is continuous.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [18](../../18.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
