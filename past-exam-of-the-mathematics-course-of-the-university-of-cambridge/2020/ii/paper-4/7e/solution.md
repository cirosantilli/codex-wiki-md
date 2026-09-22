<h1 id="7e/solution">Solution</h1>

↑ **Parent:** [7E](../7e.md)

With the stated sign convention, write $t=y-x$ to obtain

$$
\mathcal H(e^{i\omega x})(y)
=\frac{e^{i\omega y}}\pi\,\mathcal P\!\int_{-\infty}^{\infty}\frac{e^{-i\omega t}}t\,dt.
$$

The [Cauchy principal value](../../../../../cauchy-principal-value.md) of the cosine part vanishes by [oddness](../../../../../odd-function.md), while the [Dirichlet integral](../../../../../dirichlet-integral.md) gives

$$
\mathcal P\!\int_{-\infty}^{\infty}\frac{e^{-i\omega t}}t\,dt=-i\pi\operatorname{sgn}(\omega).
$$

Thus the [Hilbert transform](../../../../../hilbert-transform.md) has [Fourier multiplier](../../../../../fourier-multiplier-operator.md) $-i\operatorname{sgn}(\omega)$. Taking the real part yields

$$
\boxed{\mathcal H(\cos\omega x)(y)=\operatorname{sgn}(\omega)\sin(\omega y)}.
$$

## ↑ Ancestors (10)

1. [7E](../7e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
