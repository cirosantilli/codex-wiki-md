<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $f=\widehat\varphi$, a [Schwartz function](../../../../../../schwartz-function.md). Splitting the inverse [Fourier transform](../../../../../../fourier-transform.md) at the jump in the [Hilbert-transform Fourier multiplier](../../../../../../hilbert-transform-fourier-multiplier.md) gives

$$
\mathcal H\varphi(x)=-\frac i{2\pi}\left[\int_0^\infty e^{ix\xi}f(\xi)\,d\xi-\int_{-\infty}^0e^{ix\xi}f(\xi)\,d\xi\right].
$$

For $x\ne0$, [integration by parts](../../../../../../integration-by-parts.md) on each half-line shows

$$
\mathcal H\varphi(x)=\frac{f(0)}{\pi x}+\frac1{2\pi x}\left[\int_0^\infty e^{ix\xi}f'(\xi)\,d\xi-\int_{-\infty}^0e^{ix\xi}f'(\xi)\,d\xi\right].
$$

Both restricted [derivatives](../../../../../../derivative.md) are in $L^1$. The [Riemann-Lebesgue lemma](../../../../../../riemann-lebesgue-lemma.md) makes the bracket tend to zero as $|x|\to\infty$. Hence **the two-sided tail is**

$$
\boxed{\mathcal H\varphi(x)=\frac{\widehat\varphi(0)}{\pi x}+o(|x|^{-1}),\qquad |x|\to\infty.}
$$

Here $\widehat\varphi(0)=\int\varphi$. The [large-distance tail of the Hilbert transform](../../../../../../large-distance-tail-of-the-hilbert-transform.md) thus depends on the zeroth moment of the input. If that moment is nonzero, the $1/x$ tail proves that the output is not a [Schwartz function](../../../../../../schwartz-function.md), despite being smooth and square-integrable.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
