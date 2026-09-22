<h1 id="18/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For period two, the [Fourier series](../../../../../fourier-series-split.md) convention is

$$
f(x)=\frac{a_0}{2}+\sum_{n=1}^{\infty}\bigl[a_n\cos(n\pi x)+b_n\sin(n\pi x)\bigr].
$$

Since $f$ is an [even function](../../../../../even-function.md), every $b_n$ is zero. Also $a_0=\int_{-1}^1\cosh x\,dx=2\sinh1$. For $n\geq1$, an [antiderivative](../../../../../antiderivative.md) useful for the cosine coefficient is

$$
\int\cosh x\cos(n\pi x)\,dx=
\frac{\sinh x\cos(n\pi x)+n\pi\cosh x\sin(n\pi x)}{1+n^2\pi^2}.
$$

Evaluation at $\pm1$ gives $a_n=2(-1)^n\sinh1/(1+n^2\pi^2)$. Thus

$$
\boxed{f(x)=\sinh1\left[1+2\sum_{n=1}^{\infty}\frac{(-1)^n\cos(n\pi x)}{1+n^2\pi^2}\right]}.
$$

The periodic extension is continuous at $x=1$, so its [Fourier series](../../../../../fourier-series-split.md) converges to $\cosh1$ there. Since $\cos(n\pi)=(-1)^n$,

$$
\cosh1=\sinh1\left[1+2\sum_{n=1}^{\infty}\frac1{1+n^2\pi^2}\right].
$$

Therefore $\boxed{p=2,\ q=\pi}$, with $q=-\pi$ giving the same expression because only $q^2$ occurs. This is the $\beta=1$ case of [Fourier series of periodic hyperbolic sine and cosine](../../../../../fourier-series-of-periodic-hyperbolic-sine-and-cosine.md).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [18](../../18.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
