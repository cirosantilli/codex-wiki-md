<h1 id="h/1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For an autonomous [Lagrangian](../../../../../lagrangian.md), the [Euler-Lagrange equations](../../../../../euler-lagrange-equation.md) imply

$$
\frac d{dt}\left(\sum_{q=\theta,\phi}\dot q\frac{\partial L}{\partial\dot q}-L\right)=-\frac{\partial L}{\partial t}=0.
$$

Indeed, differentiating the expression cancels the acceleration terms, leaving $\sum_q\dot q(dL_{\dot q}/dt-L_q)-L_t$, which vanishes. Here $T$ is quadratic in the velocities, so $\sum\dot qL_{\dot q}=2T$. Thus the conserved [energy](../../../../../energy-split.md) is

$$
\boxed{H=T+V=E.}
$$

The azimuth $\phi$ is a [cyclic coordinate](../../../../../cyclic-coordinate.md). Its conjugate [momentum](../../../../../momentum-split.md) is constant:

$$
p_\phi=\frac{\partial L}{\partial\dot\phi}=\frac{Ma^2}{3}\sin^2\theta\,\dot\phi.
$$

Therefore $\boxed{\sin^2\theta\,\dot\phi=h}$ is constant as well. Physically, $p_\phi$ is the vertical component of [angular momentum](../../../../../angular-momentum.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [1](../../1.md)
3. [H](../../../h.md)
4. [2013](../../../../2013-split.md)
5. [Past exam of the options I course of the University of Oxford](../../../../split.md)
6. [Options I course of the University of Oxford](../../../../../options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
