<h1 id="3a/solution">Solution</h1>

↑ **Parent:** [3A](../3a.md)

The [function](../../../../../function-split.md) is odd, so only sine coefficients occur. For $n\geq1$,

$$
b_n=\frac2\pi\int_0^\pi(x^3-\pi^2x)\sin(nx)\,dx.
$$

Integration by parts gives

$$
\int_0^\pi x\sin(nx)\,dx=-\frac{\pi(-1)^n}{n},
$$

and

$$
\int_0^\pi x^3\sin(nx)\,dx
=-\frac{\pi^3(-1)^n}{n}+\frac{6\pi(-1)^n}{n^3}.
$$

The terms of order $1/n$ cancel, leaving

$$
b_n=\frac{12(-1)^n}{n^3}.
$$

Thus

$$
x^3-\pi^2x
=12\sum_{n=1}^{\infty}\frac{(-1)^n}{n^3}\sin(nx),
\qquad -\pi<x<\pi.
$$

The [Parseval identity](../../../../../parseval-identity.md) gives

$$
\frac1\pi\int_{-\pi}^{\pi}(x^3-\pi^2x)^2\,dx
=144\sum_{n=1}^{\infty}\frac1{n^6}.
$$

Direct integration yields

$$
\frac1\pi\int_{-\pi}^{\pi}
(x^6-2\pi^2x^4+\pi^4x^2)\,dx
=\frac{16\pi^6}{105}.
$$

Therefore

$$
\boxed{\sum_{n=1}^{\infty}\frac1{n^6}=\frac{\pi^6}{945}},
$$

as recorded in the [Fourier series of x cubed minus pi squared x](../../../../../fourier-series-of-x-cubed-minus-pi-squared-x.md).

## ↑ Ancestors (10)

1. [3A](../3a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
