<h1 id="5a/solution">Solution</h1>

↑ **Parent:** [5A](../5a.md)

Use a [power-series solution of a differential equation](../../../../../power-series-solution-of-a-differential-equation.md), $y=\sum_{n\geq0}c_nx^n$. Comparing coefficients gives

$$
(n-1)(n-2)c_n=c_{n-2},\qquad c_{-1}=c_{-2}=0.
$$

In particular $c_0=0$, while $c_1$ and $c_2$ are free. The two prescribed derivative pairs select $(c_1,c_2)=(a,0)$ and $(0,b)$. The next coefficients are $c_3=c_1/2$, $c_4=c_2/6$, $c_5=c_1/24$, $c_6=c_2/120$. Hence

$$
\boxed{y_1(x)=a\left(x+\frac{x^3}{2}+\frac{x^5}{24}+O(x^7)\right)},\qquad
\boxed{y_2(x)=b\left(x^2+\frac{x^4}{6}+\frac{x^6}{120}+O(x^8)\right)}.
$$

These are the first three nonzero terms when the respective parameter is nonzero; if $a=0$ or $b=0$, the corresponding solution vanishes identically.

For closed forms, set $y=xu$. Cancellation of the first-derivative terms reduces the equation, for $x\ne0$, to $u''-u=0$. The analytic solutions extend across zero, and their [hyperbolic cosine](../../../../../hyperbolic-cosine.md) and [hyperbolic sine](../../../../../hyperbolic-sine.md) expansions identify

$$
\boxed{y_1=ax\cosh x,\qquad y_2=bx\sinh x}.
$$

This is the [hyperbolic reduction of a regular-singular differential equation](../../../../../hyperbolic-reduction-of-a-regular-singular-differential-equation.md): although the original leading coefficient vanishes at zero, both selected [power-series solutions of a differential equation](../../../../../power-series-solution-of-a-differential-equation.md) are entire.

## ↑ Ancestors (10)

1. [5A](../5a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
