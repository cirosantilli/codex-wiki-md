<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Introduce the [null coordinates](../../../../../../characteristic-coordinate.md)

$$
\xi=t-x,\qquad\eta=t+x.
$$

Then $\Box=-4\partial_\xi\partial_\eta$, so the equation becomes

$$
u_{\xi\eta}=-\frac14u.
$$

Write the compatible boundary values as

$$
a(\xi)=u(\xi,0),\qquad b(\eta)=u(0,\eta),\qquad a(0)=b(0)=c.
$$

Twice integrating the equation gives the equivalent [Volterra integral equation](../../../../../../volterra-integral-equation.md)

$$
u(\xi,\eta)
=a(\xi)+b(\eta)-c
-\frac14\int_0^\xi\int_0^\eta u(s,r)\,dr\,ds.
$$

Let $T$ denote the double-integral operator including the factor $-1/4$, and put $g=a+b-c$. Successive approximation gives the [Neumann series](../../../../../../neumann-series.md)

$$
u=\sum_{m=0}^\infty T^mg.
$$

On a rectangle $|\xi|\leq R$, $|\eta|\leq R$,

$$
\|T^mg\|_\infty
\leq\frac{(R^2/4)^m}{(m!)^2}\|g\|_\infty.
$$

The series and its differentiated series converge locally uniformly. Since $a$ and $b$ are analytic, the sum is analytic and solves the equation and data near the origin.

If two solutions have the same data, their difference $w=Tw$. Iterating and using the same factorial estimate gives $\|w\|_\infty=0$ on every sufficiently small rectangle. This proves uniqueness. The argument is the [Analytic Goursat problem for a Klein--Gordon equation](../../../../../../analytic-goursat-problem-for-a-klein-gordon-equation.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
