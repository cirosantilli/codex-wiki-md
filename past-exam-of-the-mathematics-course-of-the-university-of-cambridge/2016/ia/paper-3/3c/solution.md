<h1 id="3c/solution">Solution</h1>

↑ **Parent:** [3C](../3c.md)

The [chain rule](../../../../../chain-rule.md) along a smooth curve is

$$
\boxed{\frac{d}{dt}f(\mathbf X(t))=\sum_{i=1}^n\frac{\partial f}{\partial x_i}(\mathbf X(t))X_i'(t)=\nabla f(\mathbf X(t))\cdot\mathbf X'(t).}
$$

Differentiating the circular parametrization gives the [tangent vector](../../../../../tangent-vector.md)

$$
\mathbf x'(t)=(-a\sin t,a\cos t)=(-y(t),x(t)).
$$

Thus the [chain rule](../../../../../chain-rule.md) turns the angular derivative of $u$ into $-yu_x+xu_y$. The given [partial differential equation](../../../../../partial-differential-equation-split.md) makes this equal to $u$, so along every portion of the circle inside the upper half-plane, $U(t)=u(\mathbf x(t))$ satisfies the [ordinary differential equation](../../../../../ordinary-differential-equation.md) $U'=U$. Its solution is $U(t)=U(t_0)e^{t-t_0}$.

For the two specified points take $a=\sqrt2$. The initial point corresponds to $t_0=\pi/4$ and the terminal point to $t_1=3\pi/4$. The entire intervening arc lies in $y>0$, so no continuation outside the domain is used. **The requested value is**

$$
\boxed{u(-1,1)=10e^{\pi/2}.}
$$

These circular [characteristic curves](../../../../../characteristic-curve.md) also show locally that the general solution has the polar-coordinate form $u(r,\theta)=C(r)e^\theta$, with $0<\theta<\pi$; there is no requirement of angular periodicity on the upper half-plane.

## ↑ Ancestors (10)

1. [3C](../3c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
