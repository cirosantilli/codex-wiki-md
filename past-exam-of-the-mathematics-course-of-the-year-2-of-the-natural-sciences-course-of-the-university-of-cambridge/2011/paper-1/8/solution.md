<h1 id="8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

Write a second-order [linear ordinary differential equation](../../../../linear-ordinary-differential-equation-split.md) in monic form $y''+P(x)y'+Q(x)y=0$. At a finite point $x_0$, an [ordinary point](../../../../ordinary-point-criterion-for-a-second-order-equation.md) has analytic $P,Q$. A singular point is a [regular singular point](../../../../regular-singular-point.md) if $(x-x_0)P$ and $(x-x_0)^2Q$ extend analytically there. A singular point failing this condition is an [irregular singular point](../../../../irregular-singular-point.md). The point at infinity is classified by the reciprocal coordinate $t=1/x$.

For the [Laguerre differential equation](../../../../laguerre-differential-equation.md), $P=1/x-1$ and $Q=\nu/x$. Thus $xP=1-x$ and $x^2Q=\nu x$ are analytic at zero, while $P$ itself is singular: zero is regular singular. Put $Y(t)=y(1/t)$. Since $y'=-t^2Y'$ and $y''=t^4Y''+2t^3Y'$, the transformed equation is

$$
Y''+\left(\frac1t+\frac1{t^2}\right)Y'+\frac\nu{t^3}Y=0.
$$

Here $tP_t=1+1/t$ is not analytic at zero, so **infinity is an irregular singular point**, for every real $\nu$.

For the [Frobenius solution](../../../../frobenius-solution.md), the lowest power $x^{\sigma-1}$ has coefficient $a_0\sigma^2$. Hence the [indicial equation](../../../../indicial-equation.md) is $\sigma^2=0$, and equating the remaining powers gives

$$
(k+1+\sigma)^2a_{k+1}+(\nu-k-\sigma)a_k=0.
$$

With the repeated root $\sigma=0$, the [Frobenius series for the Laguerre differential equation](../../../../frobenius-series-for-the-laguerre-differential-equation.md) obeys

$$
\boxed{a_{k+1}=\frac{k-\nu}{(k+1)^2}a_k.}
$$

If the series does not terminate, its consecutive term ratio is asymptotic to $x/k$, so the [ratio test](../../../../ratio-test.md) gives infinite [radius of convergence](../../../../radius-of-convergence.md). It is an [entire function](../../../../entire-function.md), even though the differential equation has a singular coefficient at zero. The repeated indicial root yields only one analytic Frobenius branch; an independent solution generally has a logarithmic term there.

For $\nu=n\geq0$, the factor $k-n$ stops the recurrence at degree $n$. With $a_0=1$ its coefficients are $a_k=(-1)^k\binom nk/k!$, giving the [Laguerre polynomials](../../../../laguerre-polynomial.md)

$$
\boxed{L_0=1,\qquad L_1=1-x,\qquad L_2=1-2x+\frac{x^2}{2},\qquad L_3=1-3x+\frac{3x^2}{2}-\frac{x^3}{6}.}
$$

The same termination argument includes $n=0$, as required for $L_0$ despite the earlier reference to positive integers.

## ↑ Ancestors (12)

1. [8](../8.md)
2. [Paper 1](../../paper-1-split.md)
3. [2011](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
