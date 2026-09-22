<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the [Fourier transform](../../../../fourier-transform-split.md) convention $\widehat f(k)=\int_{\mathbb R}f(t)e^{-ikt}dt$, with inverse factor $1/(2\pi)$. For [functions](../../../../function-split.md) in [L1 space](../../../../l1-space.md), their [convolution](../../../../convolution.md) is $h(t)=\int_{\mathbb R}f(s)g(t-s)ds$. [Fubini's theorem](../../../../fubini-s-theorem.md) applies because the absolute double [integral](../../../../integral-split.md) is $\|f\|_1\|g\|_1$. Substituting $r=t-s$ therefore proves the [convolution theorem](../../../../convolution-theorem.md):

$$
\widehat h(k)=\int_{\mathbb R}\int_{\mathbb R}f(s)g(r)e^{-ik(r+s)}drds=\widehat f(k)\widehat g(k).
$$

For the specified [rectangular pulse](../../../../rectangular-function.md), the support condition is $|t|<1$. Its [Fourier transform](../../../../fourier-transform-split.md) is

$$
\boxed{\widehat f(k)=\int_{-1}^1e^{-ikt}dt=\frac{2\sin k}k,\qquad\widehat f(0)=2.}
$$

The [convolution](../../../../convolution.md) $f*f$ is the length of the overlap of $(-1,1)$ and $(t-1,t+1)$. Thus it is the [triangular pulse](../../../../triangular-function.md)

$$
\boxed{(f*f)(t)=\begin{cases}2-|t|,&|t|<2,\\0,&|t|\geq2,\end{cases}\qquad\widehat{f*f}(k)=\frac{4\sin^2k}{k^2}.}
$$

The transform's value at zero is four, given by its continuous extension. In this convention, the [Parseval identity](../../../../parseval-identity.md) for [square-integrable functions](../../../../square-integrable-function.md) is

$$
\int_{\mathbb R}|f(t)|^2dt=\frac1{2\pi}\int_{\mathbb R}|\widehat f(k)|^2dk.
$$

For the [rectangular pulse](../../../../rectangular-function.md) the left side is two, giving the [sinc-squared integral](../../../../sinc-squared-integral.md)

$$
\boxed{\int_{-\infty}^{\infty}\frac{\sin^2k}{k^2}dk=\pi.}
$$

For the [triangular pulse](../../../../triangular-function.md), $\int|f*f|^2dt=2\int_0^2(2-t)^2dt=16/3$. Apply the same [Parseval identity](../../../../parseval-identity.md) with transform $4\sin^2k/k^2$ to obtain the [sinc fourth-power integral](../../../../sinc-fourth-power-integral.md)

$$
\boxed{\int_{-\infty}^{\infty}\frac{\sin^4k}{k^4}dk=\frac{2\pi}3.}
$$

Both integrands have removable singularities at zero and integrable tails.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [Paper 1](../../paper-1-split.md)
3. [2003](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
