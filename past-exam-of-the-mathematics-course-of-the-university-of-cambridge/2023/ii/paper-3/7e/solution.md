<h1 id="7e/solution">Solution</h1>

↑ **Parent:** [7E](../7e.md)

For

$$
w''+p(z)w'+q(z)w=0,
$$

a finite point $z_0$ is an [ordinary point](../../../../../ordinary-point-criterion-for-a-second-order-equation.md) exactly when $p$ and $q$ are [holomorphic](../../../../../holomorphic-function.md) there. It is a [regular singular point](../../../../../regular-singular-point-criterion-for-a-second-order-equation.md) exactly when

$$
(z-z_0)p(z)
\quad\hbox{and}\quad
(z-z_0)^2q(z)
$$

are holomorphic at $z_0$.

Put $\zeta=1/z$ and $W(\zeta)=w(1/\zeta)$. Direct differentiation gives

$$
w'=-\zeta^2W',
\qquad
w''=\zeta^4W''+2\zeta^3W',
$$

so the transformed equation is

$$
W''+\left(\frac2\zeta-
\frac{p(1/\zeta)}{\zeta^2}\right)W'
+\frac{q(1/\zeta)}{\zeta^4}W=0.
$$

Consequently $z=\infty$ is ordinary precisely when

$$
\frac2\zeta-\frac{p(1/\zeta)}{\zeta^2}
\quad\hbox{and}\quad
\frac{q(1/\zeta)}{\zeta^4}
$$

are holomorphic at $\zeta=0$. It is a [regular singular point at infinity](../../../../../regular-singular-point-at-infinity.md) precisely when $zp(z)$ and $z^2q(z)$ are holomorphic functions of $1/z$ near infinity.

If zero and infinity are regular singular and every nonzero finite point is ordinary, the [Laurent series](../../../../../laurent-series.md) of $p$ and $q$ can contain only the terms compatible with both endpoint bounds. Hence

$$
\boxed{p(z)=\frac az,
\qquad q(z)=\frac b{z^2}}
$$

for constants $a,b$. The equation is a [Cauchy-Euler differential equation](../../../../../cauchy-euler-equation.md). Its indicial equation is

$$
\lambda(\lambda-1)+a\lambda+b=0.
$$

For distinct roots $\lambda_1,\lambda_2$, the general solution on a domain with a chosen logarithm branch is

$$
w(z)=C_1z^{\lambda_1}+C_2z^{\lambda_2}.
$$

For a repeated root $\lambda$, the [general solution of an Euler-Cauchy equation](../../../../../general-solution-of-an-euler-cauchy-equation.md) is

$$
w(z)=z^\lambda(C_1+C_2\log z).
$$

Finally require infinity to be ordinary. In the transformed equation its coefficients become

$$
\frac{2-a}{\zeta},
\qquad
\frac b{\zeta^2}.
$$

Both are holomorphic at zero exactly when $a=2$ and $b=0$. Thus the further restriction is

$$
\boxed{p(z)=\frac2z,
\qquad q(z)=0.}
$$

## ↑ Ancestors (10)

1. [7E](../7e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
