<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The factor $1+e^{-i\xi}$ has a simple zero at $\pi$, and $L(\pi)\ne0$ makes the zero of $m$ there exactly order $N$. The [quadrature mirror filter](../../../../../../quadrature-mirror-filter.md) construction gives a high-pass symbol $m_1(\xi)=e^{-i\xi}\overline{m(\xi+\pi)}$, up to a constant phase, and

$$
\widehat\psi(\xi)=m_1(\xi/2)\widehat\varphi(\xi/2).
$$

The normalized [scaling function](../../../../../../scaling-function.md) has $\widehat\varphi(0)=1$, so $\widehat\psi$ has a zero of exactly order $N$ at zero. [Compact support](../../../../../../compact-support.md) of the [Daubechies wavelet](../../../../../../daubechies-wavelet.md) permits differentiation under its [Fourier transform](../../../../../../fourier-transform.md):

$$
\widehat\psi^{(r)}(0)=(-i)^r\int x^r\psi(x)\,dx.
$$

Hence

$$
\boxed{\int x^r\psi(x)\,dx=0\ (0\le r<N),\qquad \int x^N\psi(x)\,dx\ne0.}
$$

There are exactly $N$ [vanishing moments](../../../../../../vanishing-moment.md), rather than just at least $N$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 340](../../../paper-340-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
