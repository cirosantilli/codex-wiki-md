<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The origin is an [ordinary point](../../../../../ordinary-point-criterion-for-a-second-order-equation.md). Substitute $y=\sum_{n\geq0}a_nx^n$ into the equation and collect the coefficient of $x^n$:

$$
(n+2)(n+1)a_{n+2}+(k^2-n^2)a_n=0.
$$

Hence the [recurrence relation](../../../../../recurrence-relation.md) is

$$
\boxed{a_{n+2}=\frac{n^2-k^2}{(n+2)(n+1)}a_n,\qquad n\geq0.}
$$

There are two free initial coefficients. The independent even and odd [power series](../../../../../power-series.md) begin

$$
\begin{aligned}
y_{\rm e}(x)&=1-\frac{k^2}{2!}x^2+\frac{k^2(k^2-4)}{4!}x^4-\frac{k^2(k^2-4)(k^2-16)}{6!}x^6+\cdots,\\
y_{\rm o}(x)&=x+\frac{1-k^2}{3!}x^3+\frac{(1-k^2)(9-k^2)}{5!}x^5+\cdots.
\end{aligned}
$$

The general solution is $\boxed{y=a_0y_{\rm e}+a_1y_{\rm o}}$. As a useful independent check, the substitution $x=\sin t$ reduces the equation to $d^2y/dt^2+k^2y=0$. Thus

$$
y_{\rm e}=\cos(k\arcsin x),\qquad y_{\rm o}=\begin{cases}\sin(k\arcsin x)/k,&k\neq0,\\\arcsin x,&k=0.\end{cases}
$$

For a nonterminating parity series, $|a_{n+2}/a_n|\to1$, so the [ratio test](../../../../../ratio-test.md) in $x^2$ gives $\boxed{R=1}$. The [regular singular points](../../../../../regular-singular-point.md) at $\pm1$ explain the natural obstruction.

There is an important exception to an unconditional radius-one answer. If $k^2=m^2$ for an integer $m\geq0$, the series of parity $m$ terminates at degree $m$ and is a multiple of a [Chebyshev polynomial](../../../../../chebyshev-polynomial.md). Its [radius of convergence](../../../../../radius-of-convergence.md) is $\boxed{R=\infty}$; the other independent parity solution still has radius one. For $m=0$ the even solution is constant. Any nonzero combination containing the nonterminating solution has radius one. These are the full [power series of the Chebyshev differential equation](../../../../../power-series-of-the-chebyshev-differential-equation.md), including the terminating cases.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [8](../../8.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
