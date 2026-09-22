<h1 id="5a/solution">Solution</h1>

↑ **Parent:** [5A](../5a.md)

For

$$
y''+P(x)y'+Q(x)y=0,
$$

$x_0$ is an ordinary point when $P$ and $Q$ are analytic there, and a singular point otherwise. A singular point is regular singular when $(x-x_0)P(x)$ and $(x-x_0)^2Q(x)$ are analytic there. These are the ordinary-point and [regular-singular](../../../../../regular-singular-point-criterion-for-a-second-order-equation.md) criteria.

For [Kummer's equation](../../../../../kummer-differential-equation.md), substitute

$$
y=\sum_{m=0}^{\infty}c_mx^m.
$$

Equating the coefficient of $x^m$ gives

$$
(m+1)(m+b)c_{m+1}=(m+a)c_m.
$$

Taking $c_0=1$,

$$
\boxed{
c_m(a,b)=\frac{(a)_m}{(b)_m\,m!}},
$$

where $(a)_m=a(a+1)\cdots(a+m-1)$ is the rising factorial. Thus

$$
y_1=M(x,a,b)
=\sum_{m=0}^{\infty}\frac{(a)_m}{(b)_m\,m!}x^m.
$$

Putting $y=x^{1-b}u$ and simplifying gives

$$
xu''+(2-b-x)u'-(a-b+1)u=0.
$$

Therefore

$$
\boxed{
y_2=x^{1-b}M(x,a-b+1,2-b)}.
$$

For nonintegral $b$, the powers $x^0$ and $x^{1-b}$ at zero are distinct, so these solutions are linearly independent.

When $b\to1$, both solutions tend to $M(x,a,1)$. Differentiate their difference with respect to $b$. Writing $M_a,M_b$ for derivatives with respect to the second and third arguments,

$$
\begin{aligned}
\lim_{b\to1}\frac{y_2-y_1}{b-1}
&=-M(x,a,1)\log x\\
&\quad-M_a(x,a,1)-2M_b(x,a,1).
\end{aligned}
$$

Hence at $b=1$ one may take

$$
\boxed{
M(x,a,1),\qquad
-M(x,a,1)\log x-M_a(x,a,1)-2M_b(x,a,1)}
$$

as two linearly independent solutions. Their independence follows from the logarithmic term in the second solution.

## ↑ Ancestors (10)

1. [5A](../5a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
