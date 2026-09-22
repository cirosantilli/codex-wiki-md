<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [holomorphic function](../../../../holomorphic-function-split.md) on the [open set](../../../../open-set.md) $\Omega$ is [complex differentiable](../../../../complex-differentiability.md) at every point of $\Omega$: the [limit](../../../../limit-of-a-function.md)

$$
f'(z)=\lim_{h\to0,\ h\in\mathbb C}\frac{f(z+h)-f(z)}h
$$

exists independently of the direction of approach. Write $f(x+iy)=u(x,y)+iv(x,y)$. The [Cauchy-Riemann equations](../../../../cauchy-riemann-equations.md) are

$$
\boxed{u_x=v_y,\qquad u_y=-v_x.}
$$

To prove necessity, approach first with real $h$, obtaining $f'(z)=u_x+iv_x$. Approach instead with $h=it$ for real $t$, obtaining

$$
f'(z)=\frac1i(u_y+iv_y)=v_y-iu_y.
$$

Equality of real and imaginary parts yields the displayed [Cauchy-Riemann equations](../../../../cauchy-riemann-equations.md).

A sufficient condition is that $u$ and $v$ have continuous first [partial derivatives](../../../../partial-derivative.md) throughout $\Omega$ and satisfy the [Cauchy-Riemann equations](../../../../cauchy-riemann-equations.md) there. Indeed, real [differentiability](../../../../differentiability.md) gives, for $h=a+ib$,

$$
f(z+h)-f(z)=f_xa+f_yb+o(|h|).
$$

The [Cauchy-Riemann equations](../../../../cauchy-riemann-equations.md) imply $f_y=if_x$, so this is $f_xh+o(|h|)$. Dividing by $h$ proves [complex differentiability](../../../../complex-differentiability.md) and $f'(z)=f_x(z)$ at every point. Merely having first [partial derivatives](../../../../partial-derivative.md) and the equations at a point, without a suitable differentiability hypothesis, would not justify this argument.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [5](../../5.md)
3. [2012](../../../2012-split.md)
4. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
