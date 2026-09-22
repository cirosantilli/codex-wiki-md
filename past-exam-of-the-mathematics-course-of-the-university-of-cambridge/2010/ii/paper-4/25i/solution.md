<h1 id="25i/solution">Solution</h1>

↑ **Parent:** [25I](../25i.md)

Independence gives $S_n\sim N(0,n)$. For every integer $m$,

$$
\mathbb E e^{2\pi i mU_n}
=\mathbb E e^{2\pi i mS_n}
=e^{-2\pi^2m^2n},
$$

since subtraction of an integer does not change the exponential. These are precisely the [Fourier coefficients](../../../../../fourier-coefficient.md) of the distribution on the circle.

One can also obtain a direct density proof on $[0,1]$, avoiding an endpoint issue in transferring circle convergence. Periodize the normal density:

$$
f_n(u)=\sum_{k\in\mathbb Z}\frac1{\sqrt{2\pi n}}
e^{-(u+k)^2/(2n)},\qquad0\le u<1.
$$

Its coefficients are the displayed Gaussian values, so its absolutely convergent [Fourier series](../../../../../fourier-series-split.md) is

$$
f_n(u)=1+2\sum_{m\ge1}e^{-2\pi^2m^2n}\cos(2\pi mu).
$$

The sum of the absolute values of the nonconstant coefficients tends to zero, for example by domination by the summable sequence at $n=1$. Therefore $f_n\to1$ uniformly, and integrating any bounded continuous function on $[0,1]$ gives

$$
\boxed{U_n\ \xrightarrow{\mathrm d}\ \operatorname{Unif}[0,1].}
$$

In fact the convergence is in [total variation](../../../../../total-variation.md).

## ↑ Ancestors (10)

1. [25I](../25i.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
