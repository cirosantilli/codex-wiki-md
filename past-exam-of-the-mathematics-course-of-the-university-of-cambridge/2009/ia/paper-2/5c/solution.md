<h1 id="5c/solution">Solution</h1>

↑ **Parent:** [5C](../5c.md)

On an interval where $y>0$, the [Bernoulli differential equation](../../../../../bernoulli-differential-equation.md) is transformed by $u=y^{1-p}$:

$$
u'=(1-p)y^{-p}y'=(1-p)(f_1u+f_2).
$$

For $f_1=1$, $f_2=x$, put $s=1-p\ne0$. An [integrating factor](../../../../../integrating-factor.md) $e^{-sx}$ solves $u'-su=sx$, giving $u=Ce^{sx}-x-s^{-1}$. Thus the positive branches are

$$
\boxed{y(x)=\left(Ce^{(1-p)x}-x-\frac1{1-p}\right)^{1/(1-p)},}
$$

on intervals where the expression in parentheses is positive. The transformation omits the separate solution $y\equiv0$. For $0<p<1$, the right-hand side need not be locally [Lipschitz continuous](../../../../../lipschitz-continuity.md) at zero, so nonnegative solutions can also join zero and positive branches where the original equation permits; the formula describes every strictly positive segment.

For the autonomous case, $y'=y-\alpha^2y^p$. Its two nonnegative [equilibrium points](../../../../../equilibrium-point-of-a-dynamical-system.md) are

$$
\boxed{y=0,\qquad y_*=|\alpha|^{2/(1-p)}.}
$$

At the positive [equilibrium point](../../../../../equilibrium-point-of-a-dynamical-system.md), $f'(y_*)=1-p$. If $p>1$, $f(y)>0$ below $y_*$ and $f(y)<0$ above it; hence **$0$ is unstable and $y_*$ is asymptotically stable**. Every strictly positive solution tends to $y_*$ forward in time.

If $0<p<1$, those signs reverse: **$0$ is stable from the nonnegative side and $y_*$ is unstable**. The stability at zero follows from the phase-line signs, not a finite derivative there. For initial value $0<y_0<y_*$, the transformed equation is $u'=s(u-\alpha^2)$ with $s>0$. The solution reaches zero at

$$
T=\frac1{1-p}\log\frac{\alpha^2}{\alpha^2-y_0^{1-p}},
$$

and remains zero thereafter as a nonnegative forward solution. This is [finite-time extinction in a sublinear Bernoulli equation](../../../../../finite-time-extinction-in-a-sublinear-bernoulli-equation.md). Initial values above $y_*$ increase without bound; the sublinear negative term prevents neither that growth nor the instability of $y_*$.

## ↑ Ancestors (10)

1. [5C](../5c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
