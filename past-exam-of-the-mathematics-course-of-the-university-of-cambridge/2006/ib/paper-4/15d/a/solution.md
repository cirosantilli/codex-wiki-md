<h1 id="15d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For example, it suffices to assume $f,g\in L^1(\mathbb R)$. Indeed the absolute double integral is

$$
\int_{\mathbb R}\int_{\mathbb R}|f(t)g(x-t)|\,dt\,dx=\|f\|_1\|g\|_1<\infty.
$$

Thus [Fubini's theorem](../../../../../../fubini-s-theorem.md) permits interchange in the [Fourier transform](../../../../../../fourier-transform.md) of the [convolution](../../../../../../convolution.md). With $u=x-t$,

$$
\widehat{f*g}(\lambda)=\int\!\!\int f(t)g(x-t)e^{-i\lambda x}\,dt\,dx
=\left(\int f(t)e^{-i\lambda t}\,dt\right)\left(\int g(u)e^{-i\lambda u}\,du\right).
$$

Hence the [convolution theorem](../../../../../../convolution-theorem.md) in this normalization is

$$
\boxed{\widehat{f*g}(\lambda)=\hat f(\lambda)\hat g(\lambda).}
$$

There is no extra $2\pi$ in this formula; that factor belongs to the inverse transform and [Parseval identity](../../../../../../parseval-identity.md) for the convention being used.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [15D](../../15d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
