<h1 id="17/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For period $2$, use the [Fourier series](../../../../../fourier-series-split.md) convention

$$
f(x)\sim\frac{a_0}{2}+\sum_{n=1}^{\infty}[a_n\cos(n\pi x)+b_n\sin(n\pi x)].
$$

The [Fourier coefficients](../../../../../fourier-coefficient.md) have prefactor $1$ on $[-1,1]$. First, $a_0=\int_{-1}^{1}e^x dx=2\sinh1$. For $q=n\pi$ the useful [antiderivatives](../../../../../antiderivative.md) are

$$
\int e^x\cos(qx)dx=\frac{e^x[\cos(qx)+q\sin(qx)]}{1+q^2},\qquad
\int e^x\sin(qx)dx=\frac{e^x[\sin(qx)-q\cos(qx)]}{1+q^2}.
$$

At the endpoints $\sin(n\pi)=0$ and $\cos(n\pi)=(-1)^n$, so

$$
a_n=\frac{2(-1)^n\sinh1}{1+n^2\pi^2},\qquad
b_n=-\frac{2n\pi(-1)^n\sinh1}{1+n^2\pi^2}.
$$

Consequently, on $-1<x<1$,

$$
\boxed{e^x=\sinh1+2\sinh1\sum_{n=1}^{\infty}
\frac{(-1)^n[\cos(n\pi x)-n\pi\sin(n\pi x)]}{1+n^2\pi^2}.}
$$

The [Dirichlet-Jordan convergence theorem](../../../../../dirichlet-jordan-convergence-theorem.md) justifies equality at every point of [continuity](../../../../../continuous-function.md) of the periodic extension. At odd integers the extension has a [jump discontinuity](../../../../../jump-discontinuity.md) between $e$ and $e^{-1}$, so the series converges to their average $\cosh1$, regardless of any assigned endpoint value. This is the $\kappa=L=1$ case of the [Fourier series of a periodically extended exponential](../../../../../fourier-series-of-a-periodically-extended-exponential.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [17](../../17.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
