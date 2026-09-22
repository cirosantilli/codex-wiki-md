<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Set $l=m=g=1$. At $(\theta_1,\theta_2)=(0,0)$ the [spring](../../../../../spring.md) has $d=r$, so its [potential energy](../../../../../potential-energy.md) has zero [gradient](../../../../../gradient.md): $\partial_jV_s=k(d-r)\partial_jd=0$. The gravitational [potential energy](../../../../../potential-energy.md) has $\partial_jV_g=\sin\theta_j=0$ there. Zero [velocities](../../../../../velocity.md) therefore satisfy the [Euler-Lagrange equations](../../../../../euler-lagrange-equation.md), proving this is an [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md).

For fixed $r>0$, let $\varepsilon=\max(|\theta_1|,|\theta_2|)$ and $\delta=\theta_2-\theta_1$. The [Taylor series](../../../../../taylor-series.md) give

$$
\sin\theta_2-\sin\theta_1=\delta+O(\varepsilon^3),\qquad
\cos\theta_2-\cos\theta_1=O(\varepsilon^2).
$$

Thus, near the downward [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md), the horizontal separation is positive and

$$
d=\sqrt{\bigl(r+\delta+O(\varepsilon^3)\bigr)^2+O(\varepsilon^4)}
=r+\delta+O(\varepsilon^3).
$$

In particular, $V_s=k\delta^2/2+O(\varepsilon^4)$ and $V_g=-2+(\theta_1^2+\theta_2^2)/2+O(\varepsilon^4)$. Dropping the additive constant and terms beyond quadratic order gives the [harmonic approximation](../../../../../harmonic-approximation.md)

$$
\boxed{L_{\mathrm{quadratic}}=\frac12(\dot\theta_1^2+\dot\theta_2^2)
-\frac12\left(\theta_1^2+\theta_2^2+k(\theta_1-\theta_2)^2\right).}
$$

For physical [spring constant](../../../../../spring-constant.md) $k\geq0$, the quadratic [potential energy](../../../../../potential-energy.md) is a [positive-definite quadratic form](../../../../../positive-definite-quadratic-form.md). The downward position is therefore a [stable equilibrium in Lagrangian mechanics](../../../../../stable-equilibrium-in-lagrangian-mechanics.md), and its nearby motion admits [small oscillations](../../../../../small-oscillation.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the classical mechanics course of the University of Oxford](../../../../split.md)
6. [Classical mechanics course of the University of Oxford](../../../../../classical-mechanics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
