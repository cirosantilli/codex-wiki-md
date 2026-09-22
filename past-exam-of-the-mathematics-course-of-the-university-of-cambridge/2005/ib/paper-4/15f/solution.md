<h1 id="15f/solution">Solution</h1>

↑ **Parent:** [15F](../15f.md)

The function is odd, so its [Fourier series](../../../../../fourier-series-split.md) has no constant or cosine terms. If $\lambda=m\in\mathbb Z$, it is already a Fourier basis function: for $m>0$ the only sine coefficient is $b_m=1$; for $m<0$ it is $b_{|m|}=-1$; for $m=0$ the function is zero.

For real noninteger $\lambda$, the product-to-sum identity gives

$$
b_n=\frac2\pi\int_0^\pi\sin(\lambda x)\sin(nx)\,dx
=\frac1\pi\left[\frac{\sin((\lambda-n)\pi)}{\lambda-n}-\frac{\sin((\lambda+n)\pi)}{\lambda+n}\right].
$$

Since both numerator sines equal $(-1)^n\sin(\pi\lambda)$, the [Fourier series of a noninteger-frequency sine](../../../../../fourier-series-of-a-noninteger-frequency-sine.md) is

$$
\boxed{\sin(\lambda x)\sim\sum_{n\geq1}\frac{2(-1)^{n+1}n\sin(\pi\lambda)}{\pi(n^2-\lambda^2)}\sin(nx).}
$$

It equals the function for $-\pi<x<\pi$. At either periodic endpoint it equals the average of the two one-sided limits, namely zero; the noninteger-frequency function has a jump in its periodic extension there. Equality also holds in the square-integral sense on the full interval.

For $\lambda=1/2$, $b_n=8(-1)^{n+1}n/[\pi(4n^2-1)]$ and $\int_{-\pi}^\pi\sin^2(x/2)\,dx=\pi$. The [Parseval identity](../../../../../parseval-identity.md) for a real sine series is $(1/\pi)\int_{-\pi}^\pi f^2=\sum_{n\geq1}b_n^2$. Hence

$$
1=\frac{64}{\pi^2}\sum_{n\geq1}\frac{n^2}{(4n^2-1)^2},\qquad
\boxed{\sum_{n\geq1}\frac{n^2}{(4n^2-1)^2}=\frac{\pi^2}{64}.}
$$

## ↑ Ancestors (10)

1. [15F](../15f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
