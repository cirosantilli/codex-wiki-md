<h1 id="5c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a normalized equation

$$
y''+P(x)y'+Q(x)y=0,
$$

$x_0$ is an ordinary point when $P,Q$ are analytic there. It is a regular singular point when $(x-x_0)P(x)$ and $(x-x_0)^2Q(x)$ are analytic there. These are the [ordinary point criterion for a second-order equation](../../../../../../ordinary-point-criterion-for-a-second-order-equation.md) and [regular singular point criterion for a second-order equation](../../../../../../regular-singular-point-criterion-for-a-second-order-equation.md).

Here

$$
P(x)=\frac1x-1,\qquad Q(x)=\frac{\lambda}{x},
$$

so $x=0$ is regular singular. Seek a [power-series solution of a differential equation](../../../../../../power-series-solution-of-a-differential-equation.md)

$$
y=\sum_{n=0}^{\infty}a_nx^n.
$$

Equating the coefficient of $x^n$ gives

$$
(n+1)^2a_{n+1}+(\lambda-n)a_n=0,
$$

and hence

$$
a_{n+1}=\frac{n-\lambda}{(n+1)^2}a_n.
$$

Therefore

$$
\boxed{
a_n=a_0\frac{\prod_{j=0}^{n-1}(j-\lambda)}{(n!)^2}},
\qquad
y=a_0\sum_{n=0}^{\infty}
\frac{\prod_{j=0}^{n-1}(j-\lambda)}{(n!)^2}x^n.
$$

The series terminates exactly when $\lambda=N$ is a nonnegative integer: the factor with $j=N$ then makes $a_{N+1}=0$. Thus the polynomial solutions occur for

$$
\boxed{\lambda=0,1,2,\ldots}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5C](../../5c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
