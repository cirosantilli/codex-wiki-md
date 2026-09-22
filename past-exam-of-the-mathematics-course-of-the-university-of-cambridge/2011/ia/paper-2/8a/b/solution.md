<h1 id="8a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

With $t=1-x^2$ the [chain rule](../../../../../../chain-rule.md) gives $y'=-2xu'$ and $y''=-2u'+4x^2u''$. Substitution, initially for $x>0$, gives

$$
\boxed{t(1-t)u''+(1-t)u'+\frac14u=0.}
$$

The transformed coefficients are $P(t)=1/t$ and $Q(t)=1/[4t(1-t)]$. At $t=0$, both $tP$ and $t^2Q$ are analytic; at $t=1$, both $(t-1)P$ and $(t-1)^2Q$ are analytic. Each point is singular because a normalized coefficient has a pole, but satisfies the [regular singular point criterion for a second-order equation](../../../../../../regular-singular-point-criterion-for-a-second-order-equation.md). Thus **both points are regular singular points**.

For a [Frobenius method](../../../../../../frobenius-method.md) substitution $u=t^\rho\sum_{n\ge0}a_nt^n$, the lowest power gives the [indicial equation](../../../../../../indicial-equation.md)

$$
\rho(\rho-1)+\rho=\rho^2=0.
$$

The repeated [indicial root](../../../../../../indicial-root.md) is zero. Setting $\rho=0$ and equating the coefficient of $t^n$ gives

$$
(n+1)^2a_{n+1}+\left(\frac14-n^2\right)a_n=0,
\qquad
\boxed{a_{n+1}=\frac{n^2-\tfrac14}{(n+1)^2}a_n.}
$$

Consequently the analytic [power-series solution of a differential equation](../../../../../../power-series-solution-of-a-differential-equation.md) is

$$
u_1(t)=a_0\left(1-\frac t4-\frac{3t^2}{64}+\cdots\right).
$$

Taking $a_0=2\pi$ reproduces the [ellipse](../../../../../../ellipse.md) perimeter expansion.

For a second independent solution, normalize $u_1(0)=1$. [Reduction of order](../../../../../../reduction-of-order.md) and $P=1/t$ give

$$
u_2(t)=u_1(t)\int^t\frac{ds}{s\,u_1(s)^2}.
$$

Since $u_1(s)^{-2}=1+O(s)$, this has the [Logarithmic Frobenius solution](../../../../../../logarithmic-solution-from-a-repeated-frobenius-exponent.md) form

$$
\boxed{u_2(t)=u_1(t)\log t+v(t),\qquad v\ \text{analytic near }0.}
$$

The logarithm is $\log|t|$ on the real negative side, or a chosen [complex logarithm](../../../../../../complex-logarithm.md) on a slit complex neighborhood. Its nonzero logarithmic coefficient establishes independence. The physical perimeter is finite at $t=0$, so it selects the analytic branch rather than this logarithmic one.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [8A](../../8a.md)
3. [Section II](../../section-ii.md)
4. [Paper 2](../../../paper-2-split.md)
5. [Ia](../../../split.md)
6. [2011](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
