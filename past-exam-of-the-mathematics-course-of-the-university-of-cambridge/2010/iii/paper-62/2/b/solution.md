<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Squaring the finite geometric sum in the [Fejér kernel](../../../../../../fejer-kernel.md) gives its [Fourier series](../../../../../../fourier-series-split.md)

$$
F_n(t)=\frac1{2\pi n}\left|\sum_{j=0}^{n-1}e^{ijt}\right|^2=\frac1{2\pi}\sum_{|r|<n}\left(1-\frac{|r|}{n}\right)e^{irt}.
$$

For a fixed positive integer $k$ and $n>k$, convolution therefore gives $\sigma_n(e^{ikx})=(1-k/n)e^{ikx}$. Taking the real part,

$$
\boxed{\|\sigma_n(\cos kx)-\cos kx\|_\infty=\frac{k}{n}.}
$$

The ratio to $1/n$ is the nonzero constant $k$, even though the function is infinitely differentiable. This [Fejér saturation on a Fourier mode](../../../../../../fejer-saturation-on-a-fourier-mode.md) disproves an $o(n^{-1})$ estimate for all $C^2$ periodic functions.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 62](../../../paper-62-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
