<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

**Classification and existence.** For $y''+p(x)y'+q(x)y=0$, an [ordinary point](../../../../ordinary-point-criterion-for-a-second-order-equation.md) $x_0$ is one where $p,q$ are analytic. There are two independent analytic [power series](../../../../power-series.md) solutions, with arbitrary initial values $y(x_0),y'(x_0)$. A [regular singular point](../../../../regular-singular-point.md) is a singular point where $(x-x_0)p(x)$ and $(x-x_0)^2q(x)$ are analytic. The [Frobenius method](../../../../frobenius-method.md) then constructs solutions beginning with $(x-x_0)^\sigma$, where $\sigma$ solves the [indicial equation](../../../../indicial-equation.md). At least one [Frobenius solution](../../../../frobenius-solution.md) exists; two such solutions exist without logarithms when the two exponents differ by a noninteger. Repeated exponents or an integer difference can require a logarithmic second solution.

For this equation,

$$
xp(x)=\frac{1-x}2,\qquad x^2q(x)=-\frac x4.
$$

Both are analytic at zero, while $p,q$ themselves have poles there. Thus zero is a [regular singular point](../../../../regular-singular-point.md).

**Indicial equation and recurrence.** Multiply by $4x$ and insert $y=x^\sigma\sum_{n\geq0}a_nx^n$, $a_0\ne0$:

$$
4xy''+2(1-x)y'-y=0.
$$

The lowest power $x^{\sigma-1}$ has coefficient $[4\sigma(\sigma-1)+2\sigma]a_0$, giving

$$
\boxed{2\sigma(2\sigma-1)=0,\qquad\sigma=0,\ \frac12.}
$$

The coefficient of $x^{n+\sigma}$ is

$$
2(n+\sigma+1)(2n+2\sigma+1)a_{n+1}-(2n+2\sigma+1)a_n.
$$

For either exponent the common factor is nonzero for $n\geq0$, so the [recurrence relation](../../../../recurrence-relation.md) reduces to

$$
\boxed{a_{n+1}=\frac{a_n}{2(n+\sigma+1)},\qquad n\geq0.}
$$

Normalizing each leading coefficient to one, the two [Frobenius solutions](../../../../frobenius-solution.md) are

$$
\boxed{y_1(x)=\sum_{n=0}^\infty\frac{x^n}{2^nn!}=e^{x/2},\qquad y_2(x)=\sqrt{x}\left(1+\frac x3+\frac{x^2}{15}+\frac{x^3}{105}+\cdots\right).}
$$

More explicitly, $y_2=\sqrt{x}\sum_{n\geq0}2^nn!x^n/(2n+1)!$. The distinct leading powers establish [linear independence](../../../../linear-independence.md), so $y=C_1y_1+C_2y_2$ on the positive real side of the singular point. The displayed [exponential function](../../../../exponential-function.md) is the requested closed-form solution; substitution gives $y_1'=y_1/2,y_1''=y_1/4$, which makes the differential expression zero.

**Convergence.** For either exponent the ratio of successive terms in the coefficient [power series](../../../../power-series.md) is

$$
\left|\frac{a_{n+1}x^{n+1}}{a_nx^n}\right|=\frac{|x|}{2|n+\sigma+1|}\longrightarrow0.
$$

Thus both coefficient series have $\boxed{R=\infty}$ by the [ratio test](../../../../ratio-test.md). This does not remove the $\sqrt{x}$ branch point of $y_2$: its analytic coefficient factor is entire, while the full [Frobenius solution](../../../../frobenius-solution.md) requires a square-root branch away from zero in the complex plane. The differential equation has no other finite singular points to limit continuation of these coefficient series.

## ↑ Ancestors (12)

1. [6](../6.md)
2. [Paper 1](../../paper-1-split.md)
3. [2001](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
