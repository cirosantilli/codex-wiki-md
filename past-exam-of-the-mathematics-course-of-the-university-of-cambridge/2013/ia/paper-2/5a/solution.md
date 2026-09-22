<h1 id="5a/solution">Solution</h1>

↑ **Parent:** [5A](../5a.md)

For the normalized second-order equation, an [ordinary point](../../../../../ordinary-point-criterion-for-a-second-order-equation.md) is one where both coefficient functions $p,q$ are analytic. A [singular point of a second-order linear ODE](../../../../../singular-point-of-a-second-order-linear-ode.md) is a point that is not ordinary. It is a [regular singular point](../../../../../regular-singular-point.md) if $(x-x_0)p(x)$ and $(x-x_0)^2q(x)$ extend analytically to $x_0$; a singular point failing that condition is irregular.

Here $p=0$, $q=1/x$. Thus zero is singular but regular, because $xp=0$ and $x^2q=x$ are analytic. Write the analytic solution as $y=\sum_{n\geq0}a_nx^n$. Its constant equation gives $a_0=0$, and for $n\geq1$,

$$
n(n+1)a_{n+1}+a_n=0.
$$

Using $a_1=1$ gives

$$
\boxed{y(x)=\sum_{n=1}^\infty\frac{(-1)^{n-1}x^n}{(n-1)!n!}
=x-\frac{x^2}{2}+\frac{x^3}{12}-\frac{x^4}{144}+\cdots}.
$$

The factorial denominators show convergence for every finite $x$.

For the other branch, integrating the first correction equation twice and imposing its two conditions gives $y_1'=-\log x$ and

$$
\boxed{y_1=x-x\log x}.
$$

Then $y_2''=\log x-1$, so $y_2'=x\log x-2x+2$ and

$$
\boxed{y_2=\frac{x^2}{2}\log x-\frac{5x^2}{4}+2x}.
$$

Each correction tends to zero at the origin and its [derivative](../../../../../derivative.md) vanishes at one. Although the second solution has a finite limiting value one, it has a [logarithmically divergent endpoint derivative](../../../../../logarithmically-divergent-derivative-at-a-regular-singular-endpoint.md). Indeed the differential equation gives $y''\sim-1/x$, and integration gives

$$
\boxed{y'(x)\sim-\log x\longrightarrow+\infty\quad(x\downarrow0)}.
$$

A finite initial [derivative](../../../../../derivative.md) cannot be prescribed for this second branch. The [logarithm](../../../../../logarithm.md) is consistent with the integer separation of the two exponents in the [Frobenius method](../../../../../frobenius-method.md); this is not the repeated-exponent case.

## ↑ Ancestors (10)

1. [5A](../5a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
