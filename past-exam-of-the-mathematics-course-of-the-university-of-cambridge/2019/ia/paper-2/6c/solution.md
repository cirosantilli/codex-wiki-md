<h1 id="6c/solution">Solution</h1>

↑ **Parent:** [6C](../6c.md)

Substitute the [power series](../../../../../power-series.md) $y=\sum_{n\geq0}a_nx^n$ and compare the coefficient of $x^n$. This gives

$$
(n+2)(n+1)a_{n+2}+(\lambda^2-n^2)a_n=0,
$$

or

$$
\boxed{a_{n+2}=\frac{n^2-\lambda^2}{(n+1)(n+2)}a_n}.
$$

The two arbitrary coefficients $a_0,a_1$ determine all solutions. The condition $y'(0)=0$ sets $a_1=0$, leaving the even series. It terminates precisely when $\lambda^2=(2k)^2$ for some nonnegative integer $k$. Therefore the permitted real values are $\lambda=0$ or $\lambda=\pm2k$ for $k\geq1$; these are the even [Chebyshev polynomials](../../../../../chebyshev-polynomial.md) up to normalization.

The degrees below six occur for $\lambda=0,\pm2,\pm4$. Taking $a_0=1$, the corresponding polynomials are

$$
1,\qquad 1-2x^2,\qquad 1-8x^2+8x^4.
$$

For the forced equation, try $y=a_0+a_2x^2+a_4x^4$. Comparing the coefficients of $x^4,x^2,1$ gives

$$
-15a_4=8,
\qquad 12a_4-3a_2=0,
\qquad 2a_2+a_0=-3.
$$

Thus one polynomial satisfying $y'(0)=0$ is

$$
\boxed{y(x)=\frac{19-32x^2-8x^4}{15}}.
$$

## ↑ Ancestors (10)

1. [6C](../6c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
