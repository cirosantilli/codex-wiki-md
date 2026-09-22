<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $G(p)=\mathcal L[J_0](p)$, initially for real $p>0$. Besides the [Laplace transform of a derivative](../../../../laplace-transform-of-a-derivative.md), use multiplication by the original variable in the form

$$
\mathcal L[xg(x)](p)=-\frac d{dp}\mathcal L[g](p).
$$

Transforming the [Bessel differential equation](../../../../bessel-differential-equation.md), with its given [initial conditions](../../../../initial-condition.md), yields

$$
-\frac d{dp}\bigl(p^2G-p\bigr)+(pG-1)-G'=0.
$$

The constant terms cancel, leaving $(1+p^2)G'+pG=0$. This first-order [ordinary differential equation](../../../../ordinary-differential-equation.md) integrates to

$$
G(p)=\frac C{\sqrt{1+p^2}}.
$$

The [initial value theorem for Laplace transforms](../../../../initial-value-theorem-for-laplace-transforms.md) gives $\lim_{p\to\infty}pG(p)=J_0(0)=1$, so $C=1$. Thus the [Laplace transform of the Bessel function J0](../../../../laplace-transform-of-the-bessel-function-j0.md) is

$$
\boxed{\overline{J_0}(p)=\frac1{\sqrt{1+p^2}},\qquad p>0.}
$$

For complex $p$ with $\operatorname{Re}p>0$, choose the analytic square-root branch agreeing with the positive square root on the positive real axis.

For the forcing $k=J_0$, part (b) now gives $F(p)=(1+p^2)^{-3/2}$. On the other hand, the same multiplication rule gives

$$
\mathcal L[xJ_0(x)](p)=-G'(p)=\frac p{(1+p^2)^{3/2}}.
$$

Taking an [integral](../../../../integral-split.md) from zero divides the [Laplace transform](../../../../laplace-transform.md) by $p$. By [uniqueness of the Laplace transform](../../../../uniqueness-of-the-laplace-transform.md),

$$
\boxed{f(x)=\int_0^x tJ_0(t)\,dt.}
$$

A direct check also explains the cancellation. This expression has $f'=xJ_0$ and $f''=J_0+xJ_0'$. The [Bessel differential equation](../../../../bessel-differential-equation.md) says $(xJ_0')'=-xJ_0$, so integration from zero gives $xJ_0'=-\int_0^x tJ_0(t)\,dt=-f$. Hence $f''+f=J_0$, and both [initial conditions](../../../../initial-condition.md) hold.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the short options course of the University of Oxford](../../../split.md)
5. [Short options course of the University of Oxford](../../../../short-options-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
