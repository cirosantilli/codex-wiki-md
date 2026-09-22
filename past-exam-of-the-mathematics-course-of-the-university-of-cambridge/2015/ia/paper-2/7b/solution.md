<h1 id="7b/solution">Solution</h1>

↑ **Parent:** [7B](../7b.md)

Work on an interval where the [change of variables](../../../../../change-of-variables-formula.md) is smooth and invertible, with $s=\dot x\ne0$. If $v(t)=u(x(t))$, the [chain rule](../../../../../chain-rule.md) gives $\dot v=s u_x$ and $\ddot v=s^2u_{xx}+\dot s u_x$. Eliminating $u_{xx}$ using the original [second-order linear differential equation](../../../../../second-order-linear-differential-equation.md) gives

$$
\boxed{\ddot v-\frac{\dot s}{s}\dot v-s^2f(x)v=0.}
$$

For the real transformation as printed, take $s>0$. Set $v=s^{1/2}U$, which is the [Liouville transformation of a second-order equation](../../../../../liouville-transformation-of-a-second-order-equation.md). Differentiating twice makes the coefficient of $\dot U$ cancel. Dividing by $s^{1/2}$ leaves

$$
\boxed{\ddot U-\left[s^2f(x)+\frac{3\dot s^2}{4s^2}-\frac{\ddot s}{2s}\right]U=0.}
$$

The additional term is exactly $s^{-1/2}[(\dot s/s)d(s^{1/2})/dt-d^2(s^{1/2})/dt^2]$, as required.

On an interval with $f>0$, choose $s=f^{-1/2}$ and therefore $t=\int^x\sqrt{f(\zeta)}\,d\zeta$ up to a constant. Primes in the following expression mean derivatives with respect to $x$. We have $\dot s=-f'/(2f^2)$ and $\ddot s=-f''/(2f^{5/2})+(f')^2/f^{7/2}$, giving the [WKB correction term](../../../../../wkb-correction-term.md)

$$
\boxed{\ddot U-[1+F(t)]U=0,\qquad F(t)=\left[\frac{f''}{4f^2}-\frac{5(f')^2}{16f^3}\right]_{x=x(t)}.}
$$

Neglecting $F$ gives $U=c_+e^t+c_-e^{-t}$. Since $u=s^{1/2}U$, the [WKB approximation](../../../../../wkb-approximation.md) is

$$
\boxed{u(x)\approx f(x)^{-1/4}\left(c_+e^{\int^x\sqrt f\,d\zeta}+c_-e^{-\int^x\sqrt f\,d\zeta}\right),\qquad A(x)=f(x)^{-1/4},\quad G(x)=\int^x\sqrt f\,d\zeta.}
$$

Changing the lower integration limit only rescales the constants. Small $|F|$ is the stated local approximation criterion; rapid variation or a turning point can invalidate it, and small local residual alone need not imply uniform accuracy over an arbitrarily long interval.

The printed hypothesis only says $f\ne0$. If real $f<0$ on the interval, the printed square roots require a consistent complex branch. Equivalently a real [WKB approximation](../../../../../wkb-approximation.md) is

$$
u(x)\approx |f(x)|^{-1/4}\left[C_1\cos\left(\int^x\sqrt{|f|}\,d\zeta\right)+C_2\sin\left(\int^x\sqrt{|f|}\,d\zeta\right)\right].
$$

This supplies the oscillatory interpretation for the negative-$f$ case instead of silently assuming that the original nonzero hypothesis means positive. Smoothness through the derivatives used above and absence of zeros are required locally.

## ↑ Ancestors (10)

1. [7B](../7b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
