<h1 id="5b/solution">Solution</h1>

↑ **Parent:** [5B](../5b.md)

The [Fourier sine series](../../../../../fourier-sine-series.md) coefficients of $x$ on $(0,\pi)$ are

$$
b_n=\frac2\pi\int_0^\pi x\sin(nx)\,dx=\frac{2(-1)^{n+1}}n,
$$

by [integration by parts](../../../../../integration-by-parts.md). The odd periodic extension is piecewise smooth, so the [Fourier series](../../../../../fourier-series-split.md) converges to $x$ at every interior point. Hence

$$
\boxed{x=2\sum_{n=1}^{\infty}\frac{(-1)^{n+1}}n\sin(nx),\qquad 0<x<\pi.}
$$

To justify integration from zero, the [Fourier sine series](../../../../../fourier-sine-series.md) partial sums converge to $x$ in [L2 norm](../../../../../l2-norm.md). By the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md), integration from zero to any $x\in[0,\pi]$ has error at most $\sqrt\pi$ times that [L2 norm](../../../../../l2-norm.md) error, uniformly in $x$. Integrating the partial sums and taking the limit therefore gives

$$
\frac{x^2}{2}=2\sum_{n=1}^{\infty}\frac{(-1)^{n+1}}{n^2}(1-\cos nx).
$$

The integrated [series](../../../../../series-mathematics.md) is absolutely and uniformly convergent, since its terms are bounded by $4/n^2$. Thus the resulting [Fourier cosine series](../../../../../fourier-cosine-series.md) has

$$
\boxed{a_n=\frac{4(-1)^n}{n^2}\quad(n\ge1),\qquad a_0=8\sum_{n=1}^{\infty}\frac{(-1)^{n-1}}{n^2}.}
$$

Independently, the constant coefficient is

$$
a_0=\frac2\pi\int_0^\pi x^2\,dx=\frac{2\pi^2}{3}.
$$

Comparison yields the requested exact sum

$$
\boxed{\sum_{n=1}^{\infty}\frac{(-1)^{n-1}}{n^2}=\frac{\pi^2}{12}.}
$$

## ↑ Ancestors (10)

1. [5B](../5b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
