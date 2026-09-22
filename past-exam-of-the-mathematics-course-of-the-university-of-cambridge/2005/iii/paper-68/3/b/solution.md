<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Here $n$ is a positive [integer](../../../../../../integer.md) and $m$ is an [integer](../../../../../../integer.md) index of a [Fourier coefficient](../../../../../../fourier-coefficient.md). Split a period into $n$ intervals and set $y=nx-2\pi j$ on the $j$th interval. Periodicity and integrability give

$$
\begin{aligned}
\int_0^{2\pi}f(nx)e^{imx}\,dx
&=\frac1n\sum_{j=0}^{n-1}e^{2\pi imj/n}
\int_0^{2\pi}f(y)e^{imy/n}\,dy.
\end{aligned}
$$

For $0<|m|<n$, $\zeta=e^{2\pi im/n}$ is a [root of unity](../../../../../../root-of-unity.md) different from one and satisfies $\zeta^n=1$, so $\sum_{j=0}^{n-1}\zeta^j=(1-\zeta^n)/(1-\zeta)=0$. Therefore

$$
\boxed{\int_{\mathbb T}f(nx)e^{imx}\,dx=0\qquad(0<|m|<n).}
$$

For $m=0$ the same substitution gives $\int_{\mathbb T}f(nx)\,dx=\int_{\mathbb T}f(x)\,dx$. If the [mean](../../../../../../expected-value.md) of $f$ is zero, this last mode vanishes as well. Since the [linear span](../../../../../../linear-span.md) of the exponentials with $|m|\leq n-1$ is the space of [trigonometric polynomials](../../../../../../trigonometric-polynomial.md) of degree at most $n-1$, every pairing with that space is zero. This is the [periodic dilation annihilates low Fourier modes](../../../../../../periodic-dilation-annihilates-low-fourier-modes.md) property. The integer-index assumption is essential; the stated Fourier orthogonality would generally be false for noninteger $m$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 68](../../../paper-68-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
